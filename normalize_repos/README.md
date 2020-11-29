# Normalize GitHub Repos

This script ensures that all active repositories in the creativecommons GitHub
organization are consistent in the following ways:
* They have all the labels defined in `labels.yml` present.
* They have standard branch protections set up (with some exceptions).

This script will only update color and description of existing labels or create
new labels. It will never delete labels.


## Running the Script

1. Install [Pipenv](https://pipenv.readthedocs.io/en/latest/)
2. Navigate to the `normalize_repos` folder and run `pipenv install --dev`
3. Set the `ADMIN_GITHUB_TOKEN` environment variable with your GitHub token.
   You will need a GitHub token with admin permissions to the `creativecommons`
   GitHub organization.
4. Run the script: `pipenv run normalize_repos.py`


## Repository README

See repository README for licensing information, etc:
- [`../README.md`](../README.md)
