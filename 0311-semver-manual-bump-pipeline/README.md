fly -t tutorial set-pipeline -p semver-manual-bump-pipeline -c pipeline.yml -n -l ../../vars/git-creds.yml
fly -t tutorial unpause-pipeline -p semver-manual-bump-pipeline
fly -t tutorial trigger-job -w -j semver-manual-bump-pipeline/build
fly -t tutorial destroy-pipeline -p semver-manual-bump-pipeline