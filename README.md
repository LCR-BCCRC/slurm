# GSC Snakemake Profiles

## Installation

```bash
mkdir -p ~/.config/
git clone https://github.com/LCR-BCCRC/snakemake-profiles.git ~/.config/snakemake
```

## Usage

```bash
# Use this command on numbers for running jobs on the cluster
nice snakemake --profile numbers <targets>
# Use this command on the gphosts for running jobs locally
nice snakemake --profile gphosts --cores <cores> <targets>
```
