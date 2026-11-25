# Atividade 05 - Processo de Desenvolvimento de Software

## 1. Enquadramento do projeto

O SaborGest é uma aplicação destinada a pequenas padarias, pastelarias e estabelecimentos semelhantes, com o objetivo de facilitar a gestão de colaboradores, turnos, horas de trabalho e outras operações do estabelecimento.

Os principais utilizadores são o gerente, responsável pela gestão do estabelecimento, e os funcionários, que utilizam a aplicação para consultar informação e registar a sua atividade.

Entre as principais funcionalidades encontram-se a gestão e atribuição de turnos, o registo de entrada e saída dos funcionários e o cálculo das horas trabalhadas. O projeto inclui também funcionalidades de gestão de ausências e controlo de stock.

O desenvolvimento está dividido entre uma aplicação Web, destinada à gestão, e uma aplicação Android, destinada à utilização pelos funcionários.

O meu contributo tem incidido principalmente no desenvolvimento técnico, implementação de funcionalidades, integração dos diferentes componentes e realização de testes, em articulação com os restantes elementos do grupo.

## 2. Ponto de situação por atividade

| Atividade | Trabalho realizado | Evidência e estado | Próximo passo |
|---|---|---|---|
| Comunicação | Identificação do problema, dos perfis de utilizador e levantamento inicial dos requisitos. Foram preparadas perguntas para futuros responsáveis e funcionários de padarias ou pastelarias. | Em curso. Atividade 03 - Product Request. Ainda não foram realizadas entrevistas com utilizadores reais. | Contactar um responsável de uma padaria ou pastelaria para validar as necessidades e esclarecer regras de funcionamento. |
| Planeamento | Organização do desenvolvimento por funcionalidades e módulos. Utilização do GitHub para gerir alterações ao código através de branches e pull requests. | Em curso. Repositório GitHub do SaborGest e organização do desenvolvimento por módulos. | Rever as tarefas pendentes, estabelecer prioridades com o grupo e organizar a sequência de desenvolvimento. |
| Modelação | Definição da arquitetura técnica, estrutura da base de dados e comunicação entre a aplicação Web, a aplicação Android e a API. | Em curso. PHP, Kotlin, API REST, autenticação JWT, MariaDB/MySQL e migração `20261023_stock_management.sql`. | Rever a estrutura da base de dados e confirmar se corresponde às funcionalidades implementadas. |
| Construção | Implementação de funcionalidades de gestão de colaboradores, turnos, assiduidade, ausências, trocas de turnos e stock. Realização de testes aos módulos desenvolvidos. | Em curso. Código PHP e Kotlin, ficheiro `/web/stock.php` e 11 testes de movimentos de stock executados sem falhas. | Continuar a implementação das funcionalidades pendentes, resolver problemas e testar a integração entre os componentes. |
| Entrega e disponibilização | Desenvolvimento e testes realizados principalmente em ambiente local, utilizando XAMPP. Ainda não foi disponibilizada uma versão estável para utilização real. | Não iniciado. Aplicação em desenvolvimento num ambiente local. | Preparar uma versão de demonstração, disponibilizá-la num ambiente de teste e recolher feedback de potenciais utilizadores. |

## 3. Escolha e justificação do fluxo

O fluxo predominante no desenvolvimento do SaborGest é iterativo, uma vez que o projeto tem sido desenvolvido através de ciclos de implementação, teste, revisão e melhoria das funcionalidades existentes.

Esta escolha justifica-se por dois aspetos concretos do projeto:

- As funcionalidades têm sido desenvolvidas e revistas progressivamente. Por exemplo, a gestão de stock foi acrescentada ao projeto através de alterações à base de dados, implementação do módulo Web e realização de testes aos movimentos de stock.
- A estrutura técnica e as funcionalidades têm sido ajustadas à medida que o desenvolvimento avança, permitindo corrigir problemas e melhorar a integração entre a aplicação Web, a aplicação Android, a API e a base de dados.

O projeto também apresenta elementos de fluxo paralelo, uma vez que o desenvolvimento das diferentes componentes pode decorrer em simultâneo, desde que sejam respeitadas as dependências entre elas.

Uma alternativa seria utilizar um fluxo linear, em que todas as atividades seriam concluídas sequencialmente antes de avançar para a seguinte. No entanto, esta abordagem seria menos adequada ao SaborGest, porque as funcionalidades e a estrutura técnica têm sido ajustadas durante o desenvolvimento.

Uma limitação do fluxo escolhido é a necessidade de garantir que as alterações realizadas num módulo não provocam problemas noutros componentes. Por esse motivo, é importante realizar testes de integração e rever regularmente o código desenvolvido.

É também importante distinguir iteração de incremento. No SaborGest, a revisão e melhoria de funcionalidades já existentes representam iterações, enquanto a introdução de novas áreas, como a gestão de stock, representa um incremento de funcionalidade ao produto.

## 4. Plano das próximas tarefas

Foram definidas três tarefas para a próxima etapa do desenvolvimento do SaborGest:

| Tarefa e atividade | Responsável e data | Dependência | Resultado e critério de conclusão |
|---|---|---|---|
| Validar as necessidades e regras de funcionamento (Comunicação) | Eu, em articulação com o grupo. 16/11/2026. | Conseguir estabelecer contacto com um responsável de uma padaria ou pastelaria. | Realizar uma entrevista, registar as respostas e identificar eventuais alterações necessárias aos requisitos e regras de negócio. |
| Testar o registo de entrada e saída dos funcionários (Construção) | Eu, em articulação com o grupo. 19/11/2026. | Existência de um funcionário de teste, de um turno atribuído e da comunicação funcional entre a aplicação Android e a API. | Confirmar que um funcionário com turno atribuído consegue registar a entrada e a saída e que um funcionário sem turno atribuído não consegue efetuar esses registos. Documentar os resultados. |
| Preparar uma versão de demonstração (Entrega e disponibilização) | Grupo, com a minha participação na preparação técnica. 26/11/2026. | Conclusão dos testes das funcionalidades principais e verificação dos requisitos do ambiente de disponibilização. | Preparar uma versão de demonstração que permita executar as funcionalidades principais do SaborGest num ambiente de teste. |

As datas apresentadas correspondem a uma previsão inicial e poderão ser ajustadas de acordo com a disponibilidade do grupo e a conclusão das tarefas anteriores.

## 5. Validação de um resultado

Para a validação de uma funcionalidade, foi escolhido o requisito relacionado com o registo de entrada e saída dos funcionários.

**Funcionalidade a avaliar**

O sistema deve permitir ao funcionário registar o início e o fim do seu turno, desde que tenha um turno previamente atribuído pelo gerente.

**Participantes**

A validação será realizada pelos elementos do grupo, simulando os perfis de gerente e funcionário. Posteriormente, poderá ser repetida com potenciais utilizadores reais.

**Condições e dados de teste**

Serão utilizados dois cenários:

- Um funcionário com um turno previamente atribuído pelo gerente, que deverá conseguir registar a entrada e a saída.
- Um funcionário sem qualquer turno atribuído, que não deverá conseguir efetuar o registo de entrada ou saída.

Também será verificado se os registos ficam associados ao funcionário e ao respetivo turno.

**Resultado esperado**

O sistema deverá permitir o registo apenas aos funcionários que tenham um turno previamente atribuído. Os horários registados deverão ficar associados ao colaborador correto e permitir o cálculo das respetivas horas trabalhadas.

**Atividade transversal: Gestão de versões**

Uma atividade transversal que será aplicada ao longo do desenvolvimento é a gestão de versões.

Esta atividade será realizada através do Git e GitHub, utilizando branches para organizar alterações, commits para registar o trabalho realizado e pull requests para rever as alterações antes de serem integradas no código principal.

Desta forma, será possível acompanhar a evolução do projeto, identificar alterações, evitar conflitos entre diferentes desenvolvimentos e manter um histórico do trabalho realizado.