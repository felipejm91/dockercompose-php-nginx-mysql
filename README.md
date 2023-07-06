
<h1>DOCKER COMPOSE PARA APLICAÇÃO PHP + NGINX + MYSQL</h1>

<p>Este docker compose foi desenvolvido com o intuíto de facilitar o desenvolvimento de aplicações que utilizem PHP+MySQL+Nginx. </p>

<p><b>OBS: Esse docker compose não implementa SSL/TLS.</b></p>
<br><br>

<h2>DESCRIÇÂO PASTAS</h2><br>

* <h3>CODIGO<h3> 
<p>Nesta pasta é colocado todo o código PHP desenvolvido, pois ela será utilizada como volume no container do PHP e do Nginx.</p>

* <h3>MYSQL</h3>

Arquivo env para definição de usuário, senha e nome do banco de dados MySQL.

* <h3>Nginx</h3>

Arquivos de configuração do Nginx, sendo o arquivo default.conf as configurações para acesso à aplicação e o arquivo nginx.conf as configurações do nginx em si.

* <h3>PHP</h3>

Aqui é utilizado um dockerfile para criação de uma imagem personalizada do PHP, onde são instalados os modulos necessários para o funcionamento da aplicação. Para instalação dos módulos, insira o comando no Dockerfile:
```
RUN docker-php-ext-install nome_modulo
```

