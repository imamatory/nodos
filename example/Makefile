setup: links install

install:
	yarn

links:
	yarn --cwd ../packages/nodos-core link
	yarn --cwd ../packages/nodos-application link
	yarn --cwd ../packages/nodos-db link
	yarn --cwd ../packages/nodos-routing link
	yarn link @nodosjs/core
	yarn link @nodosjs/application
	yarn link @nodosjs/db
	yarn link @nodosjs/routing

server:
	DEBUG=nodos:* bin/nodos server -h 0.0.0.0

test:
	NODOS_ENV=test DEBUG=nodos bin/nodos test
