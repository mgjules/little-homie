sync:
	@rsync -azvh ./{traefik,docker-compose.yml} prox-eh:/home/mike

logs:
	@ssh prox-eh docker-compose logs -f

restart:
	@ssh prox-eh docker-compose restart