
up:
	docker-compose -f "docker-compose.yml" up -d --build
	docker logs --tail 1000 -f jupyter_lab
logs:
	docker logs --tail 1000 -f jupyter_lab
down:
	docker-compose -f "docker-compose.yml" down

restart:
	down
	up

