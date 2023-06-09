fly -t tutorial set-pipeline -p job-and-task-hooks -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p job-and-task-hooks
fly -t tutorial trigger-job -w -j job-and-task-hooks/job
fly -t tutorial destroy-pipeline -p job-and-task-hooks