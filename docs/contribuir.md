## [**Guia de Contribuição**](#Sumário)

Para a contribuição e evolução das informações presentes nesse repositório, o seguinte guia de contribuição foi criado, especificando instruções de uso e dos padrões utilizados.

### [**Issues**](#Sumário)

As issues devem ser criadas conforme template predefinido, contendo:

* ***Descrição*** - Descrição simples e direta do problema que a issue busca resolver ou da adição da issue;

* ***Tarefas*** - *Checklist* trazendo o passo a passo granularizado de como a issue deve ser executada, permitindo que cada tarefa seja marcada quando concluída;

* ***Critérios de Aceitação*** - *Checklist* do funcionamento ou resultado esperado após a conclusão da issue de forma satisfatória, permitindo que cada critério seja marcado quando concluído;

* ***Issue Vinculada*** - Referência a outra issue que esteja vinculada à issue presente, com link para a issue referenciada. Caso não haja issue, deve ser preenchido como 'Não se aplica.' somente;

* ***Assignees*** - As issues criadas devem ser atribuídas a um membro para execução, se houver alguém responsável por realizá-la;

* ***Labels*** - As issues criadas devem conter labels que categorizem aquela issue, para informar aos demais contribuidores sobre a natureza de seu conteúdo;

* ***Sprint*** - As issues devem possuir a sprint a qual se referem no campo destinado;

* ***Estimate*** - As issues devem ser pontuadas conforme seu grau de dificuldade;

#### **Nomenclatura**

A Nomenclatura das issues deve seguir o padrão:

```
[PREFIXO] Breve descrição da issue em português
```

De forma que o elemento **PREFIXO** siga o seguinte padrão

| Prefixo | Tema | Exemplo |
| --- | --- | --- |
| DOCS | Documentação | `[DOCS] Melhorar README`|
| DEVOPS | Integração, DevOps | `[DEVOPS] Implementar CI/CD`|
| USXX | História de Usuário, em que *XX* se refera ao número da história de usuário | `[US12] Questionário para criação de uma nova comunidade`|
| IMPROVE | Melhoria ou adição de funcionalidades não correlacionadas a uma História de Usuário | `[IMPROVE] Adiciona regras de navegação ao frontend`|


### [**Branches**](#Sumário)

Para a padronização das branches foi tomada uma adaptação do modelo padrão do [gitflow](https://nvie.com/posts/a-successful-git-branching-model/) conforme representado pelo diagrama abaixo:

![gitflow-adapted](./images-git/gitflow_adapted_tag.png)

Esse modelo segue a seguinte categorização para as respectivas branches:

* ***Main*** - A Branch *Main* contém o histórico oficial do código ou projeto em questão, sendo assim a versão do código que estará em produção no ciclo de vida do projeto.

* ***Hotfix*** - As Branches *Hotfix* servem para manutenção ou correção de forma rápida dos lançamentos em produção, feitas a partir da *Main* para uma integração mais rápida.

* ***Develop*** - A Branch *Develop* serve como uma ramificação para integração de recursos, sendo a versão do projeto disponível no ambiente de Homologação.

* ***Feature*** - As Branches de *Feature* servem para a realização de novas adições e funcionalidades para o projeto, sendo criadas a partir da branch *develop* para serem integradas a essa branch à medida que a *feature* (ou funcionalidade) em questão é concluída. Essas funcionalidades representam novas adições ao projeto em si, através da inserção de códigos.

* ***Support*** - As Branches *Support* servem para armazenar modificações que integram o projeto mas não representam funcionalidades (ou *features*), como documentação, Integração Contínua, Deploy Contínuo e demais configurações focadas na estrutura do projeto.

#### **Nomenclatura**

A Nomenclatura das branches deve seguir o seguinte padrão
 
| Branch | Nomenclatura |
| --- | --- |
| Main | main |
| Develop | develop |
| Feature | feature/<span style="color:#fc6a03">[NUMERO-USER-STORY]</span>-<span style="color:#ed820e">[BREVE-DESCRIÇÃO-EM-INGLES]</span> <br> Ex.: `feature/01-mark-point-on-map` |
| Support | support/<span style="color:#ffcd01">[BREVE-DESCRIÇÃO-EM-INGLES]</span> <br> Ex.: `support/document-contribution-guide` |
| Hotfix | hotfix/<span style="color:#cf513d">[BREVE-DESCRIÇÃO-EM-INGLES]</span> <br> Ex.: `hotfix/remove-second-callback`  |

### [**Commits**](#Sumário)

Os commits devem seguir padrões paa identificação de alterações feitas e implementadas, tanto para futuras modificações quanto para gerar rastro de informação.

#### **Nomenclatura**

A Padronização de commits foi baseada na proposta de [ConventionalCommits](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/#resumo) com adaptações, de forma que a mensagem final de commits assume a seguinte forma:

* [<span style="color:#fc6a03">#NUMERO_ISSUE</span>] <span style="color:#00c5cd">tipo</span> - <span style="color:#e11584">breve descrição em inglês, com verbo no imperativo</span>

Sendo o <span style="color:#fc6a03">**Número da Issue**</span>  o Id atribuído a ela no momento de sua criação, o <span style="color:#00c5cd">**Tipo**</span> conforme descrito na próxima sessão e a <span style="color:#e11584">Breve Descrição</span> estando na língua inglesa, contendo o verbo principal no [imperativo](https://www.infoescola.com/ingles/frases-imperativas-imperatives/), conforme o seguinte exemplo:

* [<span style="color:#fc6a03">#15</span>] <span style="color:#00c5cd">feat</span> - <span style="color:#e11584">Add user validation to point info</span>


#### **Lista de Tipos**

Os tipos de commits a serem implementados são:

* ***test***

Indica qualquer tipo de criação ou alteração de códigos de teste. Exemplo: Criação de testes unitários.

```
[#1] test - add unit test of main module
```

* ***feat***

Indica o desenvolvimento de uma nova feature ao projeto. Exemplo: Acréscimo de um serviço, funcionalidade, endpoint, etc.

```
[#2] feat - create get location function 
```

* ***refactor*** 

Usado quando houver uma refatoração de código que não tenha qualquer tipo de impacto na lógica/regras de negócio do sistema. Exemplo: Mudanças de código após um code review

```
[#3] refactor - reorder validation flow
```

* ***style*** 

Empregado quando há mudanças de formatação e estilo do código que não alteram o sistema de nenhuma forma.
Exemplo: Mudar o style-guide, mudar de convenção lint, arrumar indentações, remover espaços em brancos, remover comentários, etc..

```
[#4] style - change primary color
```

* ***fix*** 

Utilizado quando há correção de erros que estão gerando bugs no sistema.
Exemplo: Aplicar tratativa para uma função que não está tendo o comportamento esperado e retornando erro.

```
[#5] fix - remove second callback
```

* ***chore*** 

Indica mudanças no projeto que não afetem o sistema ou arquivos de testes. São mudanças de desenvolvimento.
Exemplo: Mudar regras do eslint, adicionar prettier, adicionar mais extensões de arquivos ao .gitignore

```
[#6] chore - add map library
```

* ***docs*** 

Usado quando há mudanças na documentação do projeto.
Exemplo: adicionar informações na documentação da API, mudar o README, etc.

```
[#7] docs - add architecture document
```

* ***build*** 

Utilizada para indicar mudanças que afetam o processo de build do projeto ou dependências externas.
Exemplo: Gulp, adicionar/remover dependências do npm, etc.

```
[#8] build - remove unused dependencies
```

* ***perf*** 

Indica uma alteração que melhorou a performance do sistema.
Exemplo: alterar ForEach por while, melhorar a query ao banco, etc.

```
[#9] perf - optmize validation flow
```

* ***ci*** 

Utilizada para mudanças nos arquivos de configuração de CI.
Exemplo: Circle, Travis, BrowserStack, etc.

```
[#10] ci - implement ci/cd
```

* ***revert*** 

Indica a reverão de um commit anterior.

```
[#11] revert - revert previous commit
```

### [**Pull Requests**](#Sumário)

Deve seguir o mesmo padrão de nomenclatura da issue, e os usuŕios devem se atentar a linkar a respectiva issue a ser fechada pelo pull request.

#### **Nomenclatura**

A Nomenclatura de Pull Requests deve seguir o padrão:

```
[PREFIXO] Breve descrição do Pull Request em português
```

De forma que o elemento **PREFIXO** siga o seguinte padrão

| Prefixo | Tema | Exemplo |
| --- | --- | --- |
| DOCS | Documentação | `[DOCS] Melhorar README`|
| DEVOPS | Integração, DevOps | `[DEVOPS] Implementar CI/CD`|
| USXX | História de Usuário, em que *XX* se refera ao número da história de usuário | `[US12] Questionário para criação de uma nova comunidade`|
| IMPROVE | Melhoria ou adição de funcionalidades não correlacionadas a uma História de Usuário | `[IMPROVE] Adiciona regras de navegação ao frontend`|

## [**Licença**](#Sumário)

A Licença do repositório presente é a [**Licença MIT**](https://opensource.org/licenses/MIT), de seguinte texto:

*Copyright 2021,*

*Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:*

*The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.*

*THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.*

## [**Código de Conduta**](#Sumário)

O Código de Conduta do repositório leva em conta comportamentos que favoreçam o crescimento da comunidade e respeite a individualidade de cada membro, detalhado no [documento completo](../conduta).


## Histórico de versão

|Data | Versão | Descrição | Autor(es)
| 06.05.2022 | 1.1 | Inclusão de mais informações | Marcos Nery |