fly -t tutorial set-pipeline -p golang-lib -c pipeline.yml -n
fly -t tutorial unpause-pipeline -p golang-lib
fly -t tutorial destroy-pipeline -p golang-lib
