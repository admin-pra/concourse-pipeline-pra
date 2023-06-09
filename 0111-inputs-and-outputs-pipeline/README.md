fly -t tutorial set-pipeline -p inputs-and-outputs-pipeline -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p inputs-and-outputs-pipeline 
fly -t tutorial trigger-job -w -j inputs-and-outputs-pipeline/job-pass-files
