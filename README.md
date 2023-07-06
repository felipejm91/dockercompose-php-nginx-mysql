**# DOCKER COMPOSE PARA APLICAÇÃO PHP + NGINX + MYSQL**

Este docker compose foi desenvolvido com o intuíto de facilitar o desenvolvimento de aplicações que utilizem PHP+MySQL+Nginx. 

OBS: Esse docker compose não implementa SSL/TLS

**--**

**## DESCRIÇÂO PASTAS**
--
**###CODIGO**
Nesta pasta é colocado todo o código PHP desenvolvido, pois ela será utilizada como volume no container do PHP e do Nginx.

**###MYSQL**
Arquivo env para definição de usuário, senha e nome do banco de dados MySQL

**###Nginx**
Arquivos de configuração do Nginx, sendo o arquivo default.conf as configurações para acesso à aplicação e o arquivo nginx.conf as configurações do nginx em si.

**###PHP**
Aqui é utilizado um dockerfile para criação de uma imagem personalizada do PHP, onde são instalados os modulos necessários para o funcionamento da aplicação. Para instalação das depêndencias, é utilizado o comando RUN docker-php-ext-install nome_modulo
