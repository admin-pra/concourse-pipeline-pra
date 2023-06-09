fly -t tutorial set-team --team-name devops --local-user test
fly -t devops login -c http://4.188.232.222:8080 -u test -p test --team-name devops
fly targets
fly -t devops set-pipeline -p hello-world -c pipeline.yml -n
fly -t devops unpause-pipeline -p hello-world
fly -t devops trigger-job -w -j hello-world/job-hello-world
fly -t devops destroy-pipeline -p hello-world
fly -t tutorial destroy-team --team-name platform
fly delete-target -t platform
fly targets