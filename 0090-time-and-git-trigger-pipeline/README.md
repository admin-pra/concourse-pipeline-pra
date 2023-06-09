fly -t tutorial set-pipeline -p time-and-git-trigger-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p time-and-git-trigger-pipeline
fly -t tutorial destroy-pipeline -p time-and-git-trigger-pipeline
