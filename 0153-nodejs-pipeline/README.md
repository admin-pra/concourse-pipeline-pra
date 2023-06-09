fly -t tutorial set-pipeline -p nodejs-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p nodejs-pipeline
fly -t tutorial destroy-pipeline -p nodejs-pipeline
