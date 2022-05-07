# Manual para executar a aplicação

## Passo 1 - Setup do Servidor
O primeiro passo é colocar no ar o servidor backend. 
Para tal, é necessário ter instalado [docker](https://www.docker.com/) e [docker-compose](https://docs.docker.com/compose/), utilizado para executar cada parte do projeto mais facilmente.

1. **API Gateway**
* Clonar o repositório https://github.com/fga-eps-mds/2021.2-Cartografia-social-api-gateway
* Executar, com `docker-compose up -d gateway-prod rabbitmq mongo`

2. **API Users**
* Clonar o repositório https://github.com/fga-eps-mds/2021.2-Cartografia-social-api-users
* Executar, com `docker-compose up -d user-prod`

3. **API Comunidades**
* Clonar o repositório https://github.com/fga-eps-mds/2021.2-Cartografia-social-api-comunidades
* Executar, com `docker-compose up -d comunidade-prod`
 
4. **API Mapas**
* Clonar o repositório https://github.com/fga-eps-mds/2021.2-Cartografia-social-api-mapas
* Executar, com `docker-compose up -d maps-prod`

5. **API Midias**
* Clonar o repositório https://github.com/fga-eps-mds/2021.2-Cartografia-social-api-midia
* Executar, com `docker-compose up -d midia-prod`

Com isso, todos os microsserviços estão no ar, além do broker de mensagens que cuida da comunicação entre eles, e da base de dados.
Instruções mais detalhadas individuais podem ser vistas no README de cada repositório. 

A API fica acessível a partir da porta 8000 do IP em que os comandos foram executados.

## Passo 2 - Aplicativo

Por fim, basta alterar o link da *api* no aplicativo, para que ele se comunique com o IP ou domínio correto. Isso pode ser feito no arquivo [api.js](https://github.com/fga-eps-mds/2021.2-Cartografia-social-front/blob/develop/src/services/api.js).

Finalmente, as instruções para re-compilar o aplicativo podem ser lidas no [README](https://github.com/fga-eps-mds/2021.2-Cartografia-social-front) do repositório.

Com a APK gerada, basta instalar no celular e utilizar.

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 06.05.2022 | 1.0 | Criação do documento | Marcos Nery |