# concourse-pipelines

### Prerequisites
* dockker-ce
* docker-compose

### Install Concourse using docker-compose
* Download docker-compose file
```
curl -O https://concourse-ci.org/docker-compose.yml
```
* Update CONCOURSE_EXTERNAL_URL variable in docker-compose.yml with IP address in place of localhost
* Start concourse using below command
```
docker-compose up -d
```

### Install fly

* Refer fly installation instructions from below URL.
https://concourse-ci.org/quick-start.html#install-fly
* Check fly version
```
fly --version
```

### fly login
* Fly login to connect with concourse API Server
```
fly -t tutorial login -c http://<ip-addr>:8080 -u test -p test
```

* Check `~/.flyrc` file if target has been added successfully.

* You can also check by triggering below command
```
fly status -t tutorial
```
