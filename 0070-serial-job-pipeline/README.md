fly -t tutorial set-pipeline -p serial-job-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p serial-job-pipeline
fly -t tutorial destroy-pipeline -p serial-job-pipeline