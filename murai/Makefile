sync:
	@rsync -azvh ./{.env,.env.directus,gatus,docker-compose.yml} murai:/home/mike

logs:
	@ssh murai docker-compose logs -f

restart:
	@ssh murai docker-compose restart