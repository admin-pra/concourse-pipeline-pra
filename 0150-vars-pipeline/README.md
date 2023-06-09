fly -t tutorial set-pipeline -p vars-pipeline -c pipeline.yml -n --load-vars-from var-file.yml # or use -l
fly -t tutorial unpause-pipeline -p vars-pipeline
fly -t tutorial destroy-pipeline -p vars-pipeline
