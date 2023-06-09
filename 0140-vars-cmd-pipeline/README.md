fly -t tutorial set-pipeline -p vars-cmd-pipeline -c pipeline.yml
fly -t tutorial unpause-pipeline -p vars-cmd-pipeline
fly -t tutorial trigger-job -j vars-cmd-pipeline/show-animal-names -w ## This will fail to fin vars

fly -t tutorial set-pipeline -p vars-cmd-pipeline -c pipeline.yml -v cat-name=tom -v dog-name=spike
fly -t tutorial trigger-job -j vars-cmd-pipeline/show-animal-names -w
fly -t tutorial dp -p vars-cmd-pipeline
