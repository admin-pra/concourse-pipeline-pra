fly -t tutorial set-pipeline -p semver-pipeline -c pipeline.yml -n -l ../../vars/git-creds.yml
fly -t tutorial unpause-pipeline -p semver-pipeline
fly -t tutorial trigger-job -w -j semver-pipeline/create-a-commit
fly -t tutorial destroy-pipeline -p semver-pipeline


fly -t tutorial set-pipeline -p semver-pipeline2 -c pipeline.yml -n -l ../../vars/git-creds.yml
fly -t tutorial unpause-pipeline -p semver-pipeline2
fly -t tutorial trigger-job -w -j semver-pipeline2/create-a-commit
fly -t tutorial destroy-pipeline -p semver-pipeline2