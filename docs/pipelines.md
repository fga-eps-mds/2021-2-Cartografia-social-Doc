## Pipelines de DevOps

A integração contínua funciona em todos repositórios. Para todos commits to tipo "push" e "pull_request". Realizamos os seguintes passos:


* Instalação das dependências
* Execução do lint para verificar se o código está de acordo com a folha de estilo
* Execução da suite de testes, com coleta da cobertura
* Envio da cobertura ao Coveralls 
* Scan do Sonar Cloud e envio dos resultados de teste

Se houver a integração de commits nas branches develop ou main, um deploy é feito para o ambiente de homologação, na digital ocean.

Adicionalmente. Se uma nova tag de release é gerada, após todos esses passos os arquivos do código fonte são disponibilizados na release. Juntamente com um json contentado as métricas coletadas pelo sonar cloud naquela versão. Essas métricas também são, neste passo, enviadas ao repositório de documentação. Ficando disponíveis na pasta analytics-raw-data.

O nome dos arquivos JSON se dá pelo padrão `<fga-eps-mds-YYYY_SEMESTRE_UNB-NOME_PROJETO-NOME_REPOSITORIO-DATA_HORA_RELEASE-VERSAO_RELEASE>`
Como por exemplo, `fga-eps-mds-2021-2-Cartografia-social-api-users-03-15-2022-16-52-12-v1.1.0.json`.

