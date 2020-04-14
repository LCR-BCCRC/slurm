# GSC Snakemake Profiles

## Installation

```bash
mkdir -p ~/.config/
git clone https://github.com/LCR-BCCRC/snakemake-profiles.git ~/.config/snakemake
```

## Usage

**Important:** The `remote-numbers` profile assumes you have SSH keys set up such that you can remotely log into numbers (_i.e._ `ssh n104`) without entering a password.

```bash
# Use this command on numbers for running jobs on the cluster
nice snakemake --profile numbers <targets>
# Use this command on the gphosts for running jobs locally
nice snakemake --profile gphosts --cores <cores> <targets>
# Use this command on the gphosts for submitting jobs remotely to numbers
nice snakemake --profile remote-numbers --local-cores <cores> <targets>
```
