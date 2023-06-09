fly -t tutorial set-pipeline -p put-resources-pipeline -c pipeline.yml -n -l ../../vars/git-creds.yml
fly -t tutorial unpause-pipeline -p put-resources-pipeline
fly -t tutorial trigger-job -w -j put-resources-pipeline/create-a-commit
fly -t tutorial destroy-pipeline -p put-resources-pipeline