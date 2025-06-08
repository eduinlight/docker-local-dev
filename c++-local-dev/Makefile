SHELL=/bin/bash

all: build

docker-login:
	@# make do not recognize the environment variables so you need to pass it inline
	@# Example: DOCKER_HUB_TOKEN=${DOCKER_HUB_TOKEN} make docker-login
	@docker login -u eduinlight --password-stdin <<< ${DOCKER_HUB_TOKEN}

publish-latest:
	@docker push eduinlight/c-cpp-local-dev

build:
	@docker compose build
