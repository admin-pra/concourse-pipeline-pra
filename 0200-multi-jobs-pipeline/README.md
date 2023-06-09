fly -t tutorial set-pipeline -p multi-jobs-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p multi-jobs-pipeline
fly -t tutorial destroy-pipeline -p multi-jobs-pipeline
