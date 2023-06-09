fly -t tutorial set-pipeline -p hello-world -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p hello-world
fly -t tutorial trigger-job -w -j hello-world/job-hello-world
fly -t tutorial destroy-pipeline -p hello-world