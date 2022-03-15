# <center>Metodologia do projeto e Processos

<p align="justify">
O documento de metodologia busca descrever as abordagens utilizadas durante o processo de desenvolvimento desse projeto.  Nele serão descritas quais metodologias são usadas como referência e quais métodos são adotados para o nosso contexto.
<br>
Esse documento tem como objetivo documentar as metodologias utilizadas, assim como todos os processos adotados durante o desenvolvimento do projeto. 
</p>

# Metodologias
<p align="justify">
Todas as metodologias adotadas durante esse projeto tem relação com dois princípios fundamentais do desenvolvimento ágil de software. Esses princípios são:
</p>

> * Os **indivíduos e suas interações** acima de procedimentos e ferramentas
> * A **capacidade de resposta a mudanças** acima de uma plano pré-estabelecido
>
> -- <cite> Manifesto Ágil [1] </cite>

Com base nesses princípios, foi utilizado partes de várias metodologias já conhecidas como SCRUM, Kanban e XP com o objetivo de utilizar uma metodologia que melhor adaptasse ao nosso contexto.

## 1 SCRUM

<p align="justify">
O Scrum é um framework de gerenciamento de projetos, da organização ao desenvolvimento ágil de produtos complexos e adaptativos com o mais alto valor possível, através de várias técnicas, utilizando desde o início de 1990 e que atualmente é utilizado em mais de 60% dos projetos ágeis em todo o mundo. <a href="https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)">[2]</a><br>

Essa metodologia define várias atividades que devem ocorrer durante o processo de desenvolvimento. No nosso contexto foram adotadas as seguintes atividades: Product Backlog, Sprints, Sprint Planning, Sprint Review, Daily Meeting, 
</p>

### 1.1 Product Backlog

<p align="justify">
Product backlog é um dos artefatos descritos pelo SCRUM. Esse artefato é uma lista dinâmica de requisitos do projeto, ou seja, são as atividades e limitações que o projeto deve realizar ou está sujeito para que seja bem sucedido. <a href="https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)">[2]</a><br>

No nosso contexto, essa lista de requisitos são as issues do nosso repositório. Essas issues são abstrações de cartões de tarefas que descrevem o que deve ser feito e as limitações como tempo e pessoas alocadas.
<br><br>
O único campo obrigatório na criação de uma issue padrão do Github é o título, porém, a experiência dos integrantes do projeto demostrou que issues mal escritas são mal intepretadas e resultam em entregas de baixa qualidade. Visando padronizar a criação de issues no nosso projeto, foi criado um template de criação onde é preciso definir os campos de: Descrição, Critérios de aceitação e tarefas.
<br><br>
Na descrição irá descrever a atividade da issue, inserindo informações necessárias para o entendimento. Nesse campo deve ser evitado descrições genéricas e ambíguas.

Nos critérios de aceitação deve descrever quais serão os indicadores usados para verificar a qualidade do trabalho entregue. Alguns exemplos de critérios de aceitação são: 
</p>

> * Esse documento deve conter tabela de versionamento
> * Esse documento deve conter as referências bibliográficas
> * O documento deve seguir as normas da ABNT

Por fim, as tarefas são uma lista de sub atividades que devem ser feitas para que a issue seja concluída. Essas atividades são opcionais para a criação da issue, pois nem sempre pode ser possível definí-las durante a criação de uma tarefa. Alguns exemplos de tarefas são:
> * Buscar referência 
> * Analisar os projetos de semestres anteriores

### 1.2 Sprints
<p align="justify">

Uma sprint é a unidade básica de desenvolvimento na metodologia Scrum. As sprints podem durar entre uma semana e um mês, e são um esforço dentro de uma faixa de tempo. Esse faixa de tempo deve ser relativamente curta para possibilitar entregas parciais do sistema, gerando valor e permitindo a avaliação dinâmica do trabalho. <a href="https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)">[2]</a><br>
</p>


#### 1.2.1 Sprint Planning
<p align="justify">

Sprint planning é um evento de planejamento onde será definido quais tarefas (no nosso caso issues) do product backlog serão feitas na próxima sprint. <a href="https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)">[2]</a><br>

No nosso contexto, o projeto e suas entregas macros estão definidos no plano de ensino da disciplina, sesse modo, todas as atividade e seus prazos são conhecidas, restando somente a definição dos responsáveis pela sua realização e distribuição das tarefas dentro do prazo que se tem.

Com isso em mente, são realizadas reuniões feiras para definir quais as atividades devem ser priorizadas, com base na milestones mais próxima da data atual. Uma vez definidas as atividades, são definidos os responsáveis e a data de término da sprint.
</p>

#### 1.2.2 Sprint Review
<p align="justify">
Sprint Review é um evento de validação e verificação que ocorre antes do Sprint Planning. Durante esse evento são analisadas as entregas da sprint anterior e sua qualidade. Após essa análise a atividade pode ser concluída ou pode voltar para o product backlog, associada com um pedido de correção. Durante esse evento também são discutidas dificuldades enfrentadas e pontos de melhoria para a próxima sprint. <a href="https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)">[2]</a><br>

No nosso contexto, os sprints review ocorrem em duas etapas. A etapa de validação e verificação ocorre durante a sprint, sempre que um pull request é criado. Pull Request (PR) é a abstração da entrega de uma atividade. As atividades são realizadas em um ambiente individual de desenvolvimento, esse ambiente é um clone do ambiente original onde ficam as atividades entregues e é conhecido como branches. 
<br>
Sempre que uma atividade é concluída em seu ambiente clone, é criado um pull request, isso é, um pedido para que as alterações criadas no ambiente clone vá para o ambiente original. É nessa etapa que ocorre a validação e verificação, onde os PR's serão analisados e validados antes de serem aceitos.
<br>
A segunda etapa ocorre antes da sprint review, onde são discutidas as dificuldades enfrentadas e as sugestões de melhoria para a próxima sprint.
</p>

#### 1.2.3 Daily Meeting
<p align="justify">
Na metodologia Scrum é recomendado que se realizem reuninões de status do projeto diariamente, sendo essa reunião conhecida como daily meeting. Essa reunião é sempre realizada em um mesmo horário e deve durar no máximo 15 minutos. O objetivo é deixar todos os integrantes cientes do trabalho um do outro, desse modo cada participante deve responder a três perguntas: 
<li> O que foi feito de ontem para hoje?
<li>O que planeja fazer hoje?
<li>Houve algum impedimento para a realização de suas atividades?
</p>

## 2. KANBAN
<p align="justify">
Kanban é um quadro de cartões, sendo que cada cartão representa uma atividade, onde é controlado os fluxos em que cada cartão se encontra. Esses fluxos podem ser vários, dependendo do processo em questão, mas no geral são 3 fluxos principais: "a fazer", "fazendo" e "feito". 
<br>
No nosso contexto, o kanban foi dividido em 5 fluxos: project backlog, sprint backlog, in progress, review e done. No primeiro processo é onde ficam todos os cartões de tarefas mapeados até o momento. No segundo fluxo ficam os cartões de tarefa que serão realizados na sprint atual, no terceiro fluxo ficam as cartões cuja as tarefas já foram iniciadas, no fluxo review ficam as tarefas que já foram concluídas e estão esperando por revisão de terceiros, e no último fluxo, done, ficam as tarefas que já foram revisadas e aprovadas. <a href="https://pt.wikipedia.org/wiki/Kanban">[3]</a><br>
</p>

## 3. Extreme Programming (XP)
<p align="justify">
Extreme Programming é uma metodologia com foco em agilidade de equipes e qualidade de projetos, apoiada em valores como simplicidade, comunicabilidade e feedback. Objetivando a execução de projetos dentro prazo e do orçamento, fazendo que o cliente fique satisfeito com os resultados sem que a equipe do projeto seja sobrecarregada. <a href="https://www.devmedia.com.br/extreme-programming-conceitos-e-praticas/1498">[4]</a><br>
Serão utilizados pela equipe as seguintes práticas:

<li>Pair Programing - Programação em pares com rotatividades para gestão do conhecimento
<li>Small Realeases - Pequenas entregas
<li>Código coletivo - Revesamento de Pair Programing
<li>Equipe integral - Existência de uma única equipe
</p>

### 3.1 Pair Programing ou "Programação" Pareada
<p align="justify">
Essas duas atividades buscam fazer com que todos os membros do tipo, ou a maior parte deles, tenham o sentimento de posse sobre os artefatos do projeto. E assim evitar ao máximo possível o sentimento de "Isso não foi eu que fiz, então não é problema meu".
<br>
Com o objetivo de se criar um propriedade coletiva de todos os artefaos do projeto, as atividades chaves são sempre atribuidas para mais de uma pessoa, e revisada por terceiros. Desse modo se envolve várias pessoas durante a conclusão da tarefa, difundindo conhecimento gerado e a "posse" sobre o artefato.
</p>

### 3.2 Small Realeases ou Entregas pequenas e Refatoração
<p align="justify">
Essas duas etapas buscam realizar interações curtas mantendo a qualidade. Esse objetivo é obtido reduzindo o prazo das entregas das atividades, podendo implicar na redução da qualidade do artefato entregue. Como essa redução de qualidade não é aceitável, é atividades de refatoração, onde os artefatos entregues serão retrabalhados por outros membros do projeto a fim de corrigir eventuais erros e aumentar a qualidade do artefato.
</p>

### 3.3 Códgo coletivo
<p align="justify">
A principal ideia dessa técnica é que exista um revezamento nos pares do Pair Programming, onde todos os desenvolvedores tenham a liberdade para alterar o que quiser e a qualquer momento. Isso faz com que os membros do time não precisem ficar esperando alguém autorizar para editar certa coisa que está errada fazendo com que todos ganhem tempo. O principal benefício é a refatoração constante.
</p>

### 3.4 Equipe integral
<p align="justify">
Uma equipe integral tem como objetivo a inserção de todos os envolvidos no projeto em uma equipe em si, pois para um projeto ser bem sucesso é necessário escutar todas as pessoas que estão envolvidas nele. A principal ideia da Equipe Integral é conseguir tempo disponível onde todos os envolvidos consigam se encontrar para discutir sobre o projeto. Isso entra dentro dos princípios do XP, que é a comunicação e o feedback.
</p>


## 4. Plano de comunicação
<p align="justify">
Com o objetivo de evitar problemas na comunicação dos membros e consequentemente gerar problemas nas entregas do projeto, foi pensando no plano de comunicação da equipe. Oficialmente, toda a comunicação deve ser realizada por meio de duas ferramentas, o site de hospedagem de repositórios, GitHub, e o site de vídeoconferência Jitsi. A comunicação entre professor, equipe e clientes é realizada por meio dos canais do Discord.
<br>
As tarefas são delegadas por meio de issues e pull request, e toda comunicação deve ser feita por meio de comentários nesses dois canais. Não oficialmente, os membros os membros do projeto participam de um grupo de telegram, onde são realizadas perguntas não pertinentes ao projeto.
<br>

É fortemente desencorajado a utilização de canais não oficiais para abordar temas pertinentes sobre o projeto. Isso por que se busca deixar documentado todas as atividades realizadas durante o desenvolvimento, e comunicação por canais não oficiais dificultam essa documentação. Outro motivo é que pelo fato do projeto ser livre, no sentido das quatro liberdades descritas na licença GPL v3.0, sendo elas:
<li> A liberdade de executar o projeto, para qualuqe propósito
<li> A liberdade de estudar o projeto, e adaptá-lo para suas necessidades
<li> A liberdade de redistribuir cópias do projeto
<li> A liberdade de aperfeiçoar o programa, e liberar os seus aperfeiçoamento, de modo que toda a comunidade se beneficie.
'</p>

## Bibliografia

* [1] Manifesto Ágil, Disponível em: [https://agilemanifesto.org/iso/ptbr/manifesto.html](https://agilemanifesto.org/iso/ptbr/manifesto.html)

* [2] SCRUM, Metodologia Ágil. Disponível em: [https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software)](https://pt.wikipedia.org/wiki/Scrum_(desenvolvimento_de_software))

* [3] KANBAN. Disponível em [https://pt.wikipedia.org/wiki/Kanban](https://pt.wikipedia.org/wiki/Kanban)

* [4] Extreme Programming. Disponível em [https://www.devmedia.com.br/extreme-programming-conceitos-e-praticas/1498](https://www.devmedia.com.br/extreme-programming-conceitos-e-praticas/1498)

* [O documento de metodologia do projeto SigiVilares](https://interacao-humano-computador.github.io/2019.2-SigiVilares/planejamento/Metodologia/)

* [O documento de metodologia do projeto Acacia](https://fga-eps-mds.github.io/2019.2-Acacia/#/project_methodology)


### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 11.03.2022 | 1.0 | Inclusão das metodologias utilizadas | Rafaella Junqueira |