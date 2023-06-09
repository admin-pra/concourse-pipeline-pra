fly -t tutorial set-pipeline -p time-trigger-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p time-trigger-pipeline
fly -t tutorial destroy-pipeline -p time-trigger-pipeline
