# Criação da imagem
	
	docker build -t mysql .
	
# Criação do container
	
	docker run -it --rm --name mysql -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 mysql

	docker run -d --name mysql -e MYSQL_ROOT_PASSWORD=root -e MYSQL_PASSWORD=pass -p 3306:3306 mysql

# Utilizar Container que ja existe

	docker start mysql

# Executar o container
	
	docker exec -it mysql /bin/bash
	
	mysql -u root -p

