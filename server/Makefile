postgresinit:
	sudo docker run --name postgres16 -p 5433:5433 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=password -d postgres:16-alpine
	
postgres:
	sudo docker exec -it postgres16 psql

createdb:
	sudo docker exec -it postgres16 createdb --username=root --owner=root go-chat

dropdb:
	docker exec -it postgres16 dropdb go-chat

.PHONY: postgresinit