# <center> Backlog do Produto

O Backlog de Produto ajuda a reunir e a organizar em uma lista as expectativas que o cliente tem sobre o produto. A construção do backlog faz necessário entender do funcionamento do fluxo de planejamento do produto, e após definidas as características desejadas, é montado um registro de funcionalidades a serem priorizadas e estimadas. Em suma, um backlog consiste em uma lista ordenada de tudo o que é necessário para maximizar o valor do produto, e é composta por itens que geralmente representam melhorias, correções e/ou débitos técnicos. Os épicos funcionam como módulos ou pacotes de trabalho que agregam histórias de usuários, que serão concluídas após quitarem os critérios de aceitação e, assim, o que for desenvolvido for suficiente para fazer o usuário chegar ao final da história.

## Épicos

### E01 
<!-- **Marcar pontos** -->

**Melhoria para marcação dos pontos**

Épico relacionado com as marcações de pontos e áreas no mapa. As tarefas que se encaixam nesse épico estão relacionadas com a marcação de pontos, marcação de áreas e melhora da usabilidade das marcações. Também estão relacionadas com esse épico exclusão de pontos e tarefas associadas.

### E02

**Incluir membros à comunidade virtual**

Esse épico é referente a inclusão de membros à comunidade virtual. O objetivo é que todos os membros da comunidade possam acessar os mapa da comunidade no aplicativo. Portanto o cadastro e controle de novos membro está relacionada a esse épico.

### E03
**Salvar pontos e áreas de forma offline**

Um dos objetivos do aplicativo é ser *Offline First*, ou seja, o aplicativo deve ser capaz de funcionar offline, sem a necessidade de conexão com a internet, com isso as tarefas a respeito da marcação de pontos de forma offline se relacionam com esse épico.

### E04
<!-- Para o zenhub: **Gerenciar usuários** -->
**Validar solicitação de cadastro**

Esse épico está relacionado ao gerenciamento dos usuários dentro do app e controle de permissões e acessos para determinadas ações. A diferença desse épico para o **E02 - Incluir membros à comunidade virtual** é que o **E04** é responsável pelo controle e gerenciamento dos usuários dentro do app, enquanto o **E02** é responsável por inclusão de membros à comunidade virtual.

### E05
**Exportar relatório da comunidade**

Ao criar pontos e áreas no mapa é importante a realização da exportação desses dados para que possam ser importados em outro dispositivo ou sistema. Esse épico está relacionado a essa exportação de dados, adaptação dos dados do app para dados externos e a importação de dados para o app.

### E06 
**Gerenciar dados de uma comunidade tradicional**

Similar ao épico **E04** o controle dos dados também é importante. Portanto, é responsabilidade desse épico gerenciar os dados de uma comunidade tradicional, fazer o controle de visibilidade dos dados, possíveis aprovações de dados inseridos e possíveis rejeições de dados inseridos.

### E07 
**Entrar em contato com o projeto**

É importante proporcionar ao usuário a possibilidade de contato com a equipe do projeto, para que possamos ajudar a resolver problemas e melhorar o aplicativo. Além disso alguns cadastros podem passar por uma aprovação da equipe, e o contato é importante para que a solicitação desses cadastros seja avaliada.

### E08 
**Gerenciar comunidades virtuais**

Similar aos épicos **E04** e **E06**, o gerenciamento de comunidades virtuais é importante. Portanto, é responsabilidade desse épico gerenciar os dados de uma comunidade virtual, fazer o controle de visibilidade dos dados, controle de permissões dentro de uma comunidade e controle de visibilidade dos dados da comunidade. A diferença desse épico para os outros é que o **E08** é responsável por gerenciar os dados de uma comunidade virtual, enquanto os outros são responsáveis pelos usuários e os dados da comunidade.

### E09
**Gerenciar histórico de acesso e permissões de usuário**

É responsabilidade desse épico gerenciar o histórico de acesso e permissões de usuário, fazer o controle de visibilidade dos dados, controle de permissões dentro de uma comunidade e controle de visibilidade dos dados da comunidade. Esse épico é importante para realizações de [auditoria](https://pt.wikipedia.org/wiki/Auditoria#:~:text=Auditoria%20%C3%A9%20um%20exame%20cuidadoso,conformidade) de dados, e ter uma visibilidade das ações que foram realizadas dentro do aplicativo.

### E10

**Salvar mídias de forma offline**

Similar ao **E03**, este épico também se relaciona ao objetivo do aplicativo em ser *Offline First*. Tarefas ligadas à inserção de mídias sem o uso de internet se relacionam com esse épico.

### E11
**Exportar marcações da comunidade**

Similar ao **E05**, este épico diz respeito à exportação dos dados inseridos em uma comunidade, porém, se restringe aos dados cartográficos. 


## Histórias de Usuário 

| ID | Eu, como... | Gostaria de...  | Para poder...  | Épico |
|:--:|--|--|--|:--:|
| US01 | Usuário | Conseguir marcar no mapa os locais conforme eu me locomovo pelo terreno da minha comunidade | Delimitar as áreas de risco para a comunidade | E01 |
| US02 | Líder da comunidade virtual | Adicionar membros à comunidade virtual | Permitir que elas também possam marcar pontos e áreas referentes a um determinado território | E02 |
| US03 | Usuário | Marcar pontos e áreas sem ter conexão com a internet | Delimitar áreas em locais que não possuem sinal | E03 |
| US04 | Usuário | Me cadastrar no aplicativo | Contribuir com o projeto Nova Cartografia Social | E04 |
| US05 | Pesquisador | Exportar informações sobre uma comunidade | Manter registro das pessoas dessa comunidade | E05 |
| US06 | Pesquisador | Exportar dados geográficos detalhados spbre uma comunidade | Manter registro dos territórios dessa comunidade | E11 |
| US07 | Mantenedores | Validar o cadastro de novos usuários | Permitir o acesso de novos membros à uma comunidade virtual | E04 |
| US08 | Líder da comunidade virtual | Validar os dados inseridos por membros de uma comunidade virtual sobre um território | Garantir a acurácia dos dados que serão apresentados no aplicativo |  E06 |
| US09 | Usuário | Criar, ler, atualizar e excluir dados sobre uma comunidade virtual | Gerenciar corretamente os dados | E06 |
| US10 | Usuário | Contatar a equipe do Cartografia Social | Me comunicar com os mantenedores do projeto | E07 |
| US11 | Mantenedor | Cadastrar uma comunidade virtual no aplicativo | Marcar pontos e áreas no mapa sobre um território de comunidade tradicional | E08 |
| US12 | Mantenedor | Verificar quem acessou as comunidades virtuais e com qual tipo de permissão de usuário | Garantir a segurança das informações | E09 |
| US13 | Usuário | Editar as informações do meu perfil | Manter minhas informações atualizadas | E04 |
| US14 | Líder da comunidade virtual | Ver quem marcou pontos e áreas no aplicativo | Controlar a inserção de dados e manter a rastreabilidade de origem das informações | E09 |
| US15 | Pesquisador | Exportar mídias referentes a uma comunidade virtual | Manter registro midiáticos dessa comunidade | E05 |
| US16 | Usuário | Inserir fotos, áudios e/ou vídeos sem ter conexão com a internet | Salvar mídias em locais que não possuem sinal | E10 |


## Critérios de Aceitação

### US01
- Critério 1
- Critério 2
- ...
  
### US02
- Critério 1
- Critério 2
- ...

### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 09.03.2022 | 1.0 | Adição das Histórias de usuário e dos épicos  | Rafaella Junqueira <br> Larissa Sales |
| 10.03.2022 | 1.1 | Adição das descrições dos épicos | Gustavo Marques |
| 10.03.2022 | 1.2 | Refatoração dos épicos | Rafaella Junqueira <br> Larissa Sales |