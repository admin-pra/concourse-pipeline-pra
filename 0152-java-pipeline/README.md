fly -t tutorial set-pipeline -p java-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p java-pipeline
fly -t tutorial destroy-pipeline -p java-pipeline
