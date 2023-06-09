fly -t tutorial set-pipeline -p job-inputs-scripts -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p job-inputs-scripts
fly -t tutorial trigger-job -w -j job-inputs-scripts/job-test-app
