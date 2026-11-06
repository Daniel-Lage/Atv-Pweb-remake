Criado a pasta

Criado o html

Usado um comando no Docker para direcionar todas as requisições de uma porta específica para a porta do Docker

`docker run -d --name aula-apache -p 8080:80 -v "${PWD}:/usr/local/apache2/htdocs/" httpd:2.4`

Para conferir se está ativo: `docker ps`

Criada o arquivo "sobre.html" para referenciar a rota na url

Foi encerrado a aplicação por meio do comando `docker container rm /aula-apache`

E a porta foi trocada para 8000:80 pelo comando: `docker run -d --name aula-apache -p 8000:80 -v "${PWD}:/usr/local/apache2/htdocs/" httpd:2.4`

Para verificar as configurações do servidor `curl -v http://localhost:xxxxx/`