fly -t tutorial set-pipeline -p git-trigger-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p git-trigger-pipeline
fly -t tutorial destroy-pipeline -p git-trigger-pipeline