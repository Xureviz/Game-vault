compose = docker-compose -f docker-compose.yml

.PHONY: build
build: ##@development Build development environment.
	$(compose) build

.PHONY: up
up: build ##@development Starts development environment in background.
	$(compose) up

.PHONY: restart
restart: ##@development Restarts development environment.
	$(compose) restart

.PHONY: logs
logs: ##@development Follows development logs.
	$(compose) logs -f --tail=100

.PHONY: clean
clean: ##@development Stop development environment.
	$(compose) down --volumes --remove-orphans