fly -t tutorial execute -c no_inputs.yml
fly -t tutorial e -c inputs_required.yml && { echo "Should have failed"; exit 1; }
fly -t tutorial e -c inputs_required.yml -i some-important-input=.
fly -t tutorial e -c inputs_required.yml -i some-important-input=../.
fly -t tutorial execute -c input_parent_dir.yml

