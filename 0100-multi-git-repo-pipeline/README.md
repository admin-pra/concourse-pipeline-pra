fly -t tutorial set-pipeline -p multi-git-repo-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p multi-git-repo-pipeline
fly -t tutorial destroy-pipeline -p multi-git-repo-pipeline
