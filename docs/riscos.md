# <center> Plano de Gerenciamento de Riscos

## Introdução
O Plano de Gerenciamento de Riscos é um documento que visa entender os riscos passíveis de acometer o projeto e quais medidas tomar para evitá-los ou minimizá-los.

## Objetivo
O objetivo desse planejamento é documentar os riscos associados ao desenvolvimento do projeto e as ações que devem ser tomadas para que eles sejam reduzidos ou evitados.

## Estrutura Analítica dos Riscos
Uma forma comum para estruturar categorias dos riscos é através da EAR (Estrutura Analítica dos Riscos), que constiste em uma representação hierárquica de possíveis fontes de riscos. Uma EAR ajuda a equipe responsável pelo projeto a considerar toda as possíveis fontes das quais podem surgir cada um dos riscos do projeto.


<figcaption><center>
    <b>Figura 1 - EAR do projeto</b>
</figcaption>

[<div align="center"><img width="auto" height="auto" src="../img/organizacao/ear.png"/></div>](../../img/organizacao/ear.png)

### Riscos Técnicos

| Tipo | Descrição |
| -- | -- |
| Tecnologia | Riscos gerados a partir das tecnologias empregadas |
| Requisitos | Riscos gerados a partir da má elicitação dos requisitos |
| Qualidade | Riscos gerados a partir da baixa qualidade do produto final |
| Complexidade | Riscos gerados a partir da dificuldade de implementação por parte do time de desenvolvimento |

### Riscos Externos

| Tipo | Descrição |
| -- | -- |
| Cliente | Riscos gerados a partir das atividades relacionadas ao cliente, como mudança de escopo ou falta de validação das entregas |
| Pandemia | Riscos gerados a partir do cenário mundial atual de COVID-19 |

### Riscos de Gestao

| Tipo | Descrição |
| -- | -- |
| Planejamento | Riscos gerados a partir do mau planejamento durante o desenvolvimento do projeto |
| Comunicação | Riscos gerados a partir da comunicação não efetiva entre os as partes integrantes do projeto |
| Estimativa | Riscos gerados a partir do cronograma mal estruturado |

### Riscos da Organização

| Tipo | Descrição |
| -- | -- |
| Priorização | Riscos gerados a partir da priorização errada dos entregáveis |
| Recursos | Riscos gerados a partir do mau planejamento de custos |
| Dependências | Riscos gerados a partir da interação incorreta entre as possíveis variáveis necessárias para a entrega do projeto |

## Critérios

Os critérios abaixo foram baseados na matriz de risco descrita por Garvey e Lansdowne (1998).

### Análise de Probabilidade

Estimação da ocorrência do risco.

| Probabilidade | Intervalo |
| -- | -- |
| Muito Baixa | 0-10% |
| Baixa | 11-40% | 
| Moderada | 41-60% |
| Alta | 61-90% | 
| Muito Alta | 91-100% | 

### Análise de Impacto

Estimação do impacto do risco para o projeto.

| Impacto | Descrição |
| -- | -- |
| Mínimo | Impacto insignificante para o andamento do projeto |
| Pequeno | Impacto com pouca influência no andamento do projeto |
| Moderado | Impacto notável para o andamento do projeto |
| Sério | Impacto grave para o andamento do projeto |
| Crítico | Impacto crítico para o andamento do projeto |

### Análise de Nível

Resultado da Composição do impacto do risco com a probabilidade da sua ocorrência.

| Probabilidade / Impacto | Mínimo | Pequeno | Moderado | Sério | Crítico | 
| -- | -- | -- | -- | -- | -- |
| **Muito Alta** | Elevado | Elevado | Extremo | Extremo | Extremo 
| **Alta** | Médio | Elevado | Elevado | Extremo | Extremo | 
| **Moderada** | Baixo | Médio | Elevado | Extremo | Extremo | 
| **Baixa** | Baixo | Baixo | Médio | Elevado | Extremo | 
| **Muito Baixa** | Baixo | Baixo | Médio | Elevado | Elevado | 

## Levantamento de Riscos
| ID | Hipótese | Motivo | Consequência | EAR |
|---|---|---|---|---|
| R01 | O projeto não atender aos requisitos | Levantamento de requisitos mal elaborado ou falta de validação contínua | Atraso na entrega e nova definição dos requisitos | Requisitos |
| R02 | Baixa qualidade do produto final | Entregas ruins do time de desenvolvimento | Refatoração do produto | Qualidade |
|  | Time de desenvolvimento com dificuldades de aplicar as tecnologias | Falta de conhecimento das tecnologias | Não entrega do produto | Complexidade |
|  | Dificuldade em realizar testes na aplicação | Falta de conhecimento em testes | Atraso na entrega das histórias | Complexidade |
|  | Não automatização de deploy ou integração contínua | Falta de conhecimento | Atraso nas entregas em ambiente de produção | Complexidade |
|  | Não planejamento e execução seguindo a proposta de arquitetura | Falta de conhecimento nas tecnologias | Atraso no desenvolvimento | Complexidade |
|  | Cancelamento do projeto | Interrupção do projeto que deu origem ao desenvolvimento do aplicativo (Nova Cartografia Social da Amazônia) | Cancelamento do projeto | Cliente |
|  | Interrupção das aulas/projeto | Nova onda de contaminações por causa do COVID-19 | Cancelamento do projeto | Pandemia |
|  | Mal planejamento das histórias de usuário | Mal planejamento da sprint | Atraso na entrega do produto | Planejamento |
|  | Mudança no escopo do projeto | Mal planejamento do backlog | Atraso na entrega do produto | Planejamento |
|  | Falta de comunicação efetiva entre os membros da equipe | Não utilização dos meios de comunicação estabelecidos | Falta de alinhamento entre a equipe | Comunicação |
|  | Abandono do projeto por parte de membros da equipe | Necessidade de trancamento da matéria | Atraso na entrega do produto | Recursos |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

## Medidas de Gerência e Mitigação
| ID | Impacto | Probabilidade | Nível | Mitigação |

## Referências

TERLIZZI, Marco Alexandre & BIANCOLINO, César Augusto. Estrutura Analítica de Riscos em Projetos de Desenvolvimento de Software no Setor Bancário: Um Estudo Exploratório. **Revista Gestão & Tecnologia**, v. 14, n. 2, p. 51-78, mai./ago. 2014. Disponível em: <<http://revistagt.fpl.emnuvens.com.br/get/article/viewFile/628/534#:~:text=A%20EAR%20(Estrutura%20Anal%C3%ADtica%20de,gest%C3%A3o%20(Hillson%2C%202003)>>. Acesso em: 12 de mar de 2022.

ISOTANI, Seiji & ROCHA, Rafaela V. **Gestão de Riscos em Projetos de Software**. USP. Disponível em: <<https://edisciplinas.usp.br/pluginfile.php/3385127/mod_resource/content/1/Aula10-GerenciaProjeto-Riscos.pdf>>. Acesso em: 12 de mar de 2022.

Lansdowne Z. F. (1999), Risk matrix: an approach for prioritizing risks and tracking risk litigation
progress; Proceedings of the 30th Annual Project Management Institute Seminars & Symposium.

VELOSO, Lee. Matriz de Risco: veja as principais etapas para aplicá-la! **MOKI**, 2021. Disponível em: <<https://site.moki.com.br/matriz-de-risco/#:~:text=Como%20funciona%20a%20matriz%20de%20risco%3F,devem%20ter%20prioridade%20de%20tratamento.>>. Acesso em: 12 de mar de 2022.

JUNCKES, Gabriel Dias & MORGADO, Paulo. Gerência de riscos em desenvolvimento de software. **DEVMEDIA**, 2013. Disponível em: <<https://www.devmedia.com.br/gerencia-de-riscos-em-desenvolvimento-de-software/28506>>. Acesso em: 12 de mar de 2022.
## Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 12.03.2022 | 1.0 | Criação do documento | Larissa Sales |

