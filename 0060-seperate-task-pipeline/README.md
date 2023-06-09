fly -t tutorial set-pipeline -p seperate-task-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p seperate-task-pipeline
fly -t tutorial destroy-pipeline -p seperate-task-pipeline