fly -t tutorial set-pipeline -p passing-artifacts-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p passing-artifacts-pipeline
fly -t tutorial destroy-pipeline -p passing-artifacts-pipeline
