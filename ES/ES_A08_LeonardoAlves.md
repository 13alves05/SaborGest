# Atividade 08 - Metodologias AGILE

## Parte A - Compreensão dos conceitos

### Extreme Programming

#### 1. Origem e motivação de XP

O Extreme Programming (XP) surgiu na década de 1990, tendo sido utilizado inicialmente num projeto da Chrysler, nos Estados Unidos, com o envolvimento de Kent Beck. O seu principal objetivo é melhorar a qualidade do software e a forma como a equipa trabalha.

Dois dos seus valores são:

- **Comunicação:** permite que os elementos da equipa partilhem informação, esclareçam dúvidas e evitem mal-entendidos durante o desenvolvimento.
- **Feedback:** permite receber opiniões e identificar problemas regularmente, para fazer melhorias no software ao longo do projeto.

#### 2. TDD, programação a pares e refatorização

O TDD (Test-Driven Development) é uma forma de desenvolver software em que os testes são criados antes do código. O processo funciona em três passos: escrever um teste que inicialmente falha, desenvolver o código necessário para o fazer passar e, por fim, melhorar o código sem alterar o seu comportamento. Este ciclo repete-se ao longo do desenvolvimento.

A programação a pares consiste em dois programadores trabalharem juntos no mesmo código, permitindo partilhar conhecimentos e detetar erros mais facilmente.

A refatorização consiste em melhorar a organização e a estrutura do código, sem alterar aquilo que a funcionalidade faz. Ajuda a evitar código repetido e torna a aplicação mais fácil de manter.

#### 3. Spike

Um spike é uma tarefa de curta duração utilizada para investigar uma dúvida ou testar uma solução antes de avançar com o desenvolvimento. É útil quando a equipa não tem informação suficiente para tomar uma decisão técnica.

Por exemplo, no SaborGest, poderia ser necessário esclarecer se a aplicação Android consegue comunicar corretamente com a API REST utilizando autenticação JWT.

- **Pergunta:** como garantir que a aplicação Android consegue comunicar com a API utilizando um token JWT?
- **Limite de tempo:** um dia de trabalho.
- **Resultado esperado:** realizar um pequeno teste de comunicação e registar a solução encontrada, incluindo possíveis problemas e a decisão sobre como implementar essa ligação.

### Scrum

#### 4. Responsabilidades no Scrum

No Scrum existem três responsabilidades principais:

- **Product Owner:** é responsável por maximizar o valor do produto, definir prioridades e gerir eficazmente o Product Backlog, garantindo que o trabalho realizado corresponde às necessidades mais importantes.
- **Scrum Master:** ajuda a equipa a compreender e aplicar o Scrum, acompanha o processo e ajuda a resolver obstáculos que dificultam o desenvolvimento.
- **Developers:** são responsáveis por desenvolver o produto, organizar o trabalho de cada Sprint e garantir a qualidade das funcionalidades entregues.

A equipa pode colaborar com o cliente através de reuniões e demonstrações regulares, apresentando o trabalho realizado, esclarecendo dúvidas e recebendo opiniões que possam ajudar a definir as próximas prioridades.

#### 5. Sprint e respetivos backlogs

Uma Sprint é um período de trabalho com uma duração definida, durante o qual a equipa procura desenvolver um conjunto de funcionalidades. A sua duração máxima é de um mês.

O Product Backlog é a lista geral de funcionalidades, melhorias e tarefas necessárias para o produto, organizadas por prioridade.

O Sprint Backlog contém o objetivo da Sprint, os itens do Product Backlog selecionados para esse período e o plano de trabalho definido pelos Developers para os desenvolver.

O Sprint Goal é o objetivo principal da Sprint. Serve para manter a equipa focada no resultado que pretende alcançar durante esse período.

#### 6. Eventos Scrum

- **Daily Scrum:** reunião diária, normalmente com 15 minutos, em que os Developers verificam o progresso em relação ao objetivo da Sprint e organizam o trabalho seguinte.
- **Sprint Review:** serve para apresentar e avaliar o resultado do trabalho realizado com o cliente ou outras pessoas interessadas, recolhendo opiniões e identificando possíveis alterações.
- **Sprint Retrospective:** serve para a equipa analisar a forma como trabalhou, perceber o que correu bem e identificar o que pode melhorar.

Por exemplo, numa Sprint do SaborGest, a Review poderia servir para demonstrar o registo de entrada e saída dos funcionários. Na Retrospective, a equipa poderia analisar se a divisão das tarefas e a comunicação entre os elementos funcionaram bem.

### Kanban

#### 7. Origem e objetivo de Kanban

O Kanban tem origem no sistema de produção da Toyota, no Japão, estando associado ao trabalho de Taiichi Ohno. Mais tarde, a sua utilização foi adaptada ao desenvolvimento de software e a outras áreas de trabalho.

O seu principal objetivo é melhorar a organização e o fluxo das tarefas, permitindo perceber o que está por fazer, o que está em desenvolvimento e o que já foi concluído.

No entanto, Kanban não consiste apenas em utilizar um quadro com tarefas. Também implica definir as etapas do trabalho, controlar a quantidade de tarefas em simultâneo, identificar bloqueios e procurar melhorar continuamente a forma como a equipa trabalha.

#### 8. WIP

WIP significa Work In Progress, ou seja, trabalho que já foi iniciado, mas ainda não foi concluído.

Limitar o WIP significa definir um número máximo de tarefas que podem estar em desenvolvimento numa determinada etapa. Isto evita que os elementos da equipa comecem demasiadas tarefas ao mesmo tempo e acabem por deixar várias por terminar.

Quando uma etapa atinge o limite definido, a equipa não deve iniciar mais tarefas nessa etapa. Deve concentrar-se em concluir o trabalho existente ou resolver os problemas que estejam a bloquear o seu progresso.

#### 9. Scrum, Kanban e XP

O Scrum organiza o trabalho através de períodos definidos chamados Sprints, com reuniões e objetivos estabelecidos para cada período.

O Kanban permite gerir o trabalho de forma contínua, sem obrigar a equipa a trabalhar em períodos fixos. As tarefas vão sendo iniciadas à medida que existe capacidade disponível, respeitando os limites de WIP.

Uma prática de XP que pode complementar qualquer uma destas abordagens é a programação a pares. Dois elementos trabalham juntos na mesma funcionalidade, permitindo rever o código durante o desenvolvimento, partilhar conhecimentos e reduzir a possibilidade de erros.

## Parte B - Aplicação ao projeto de PdS (SaborGest)

### Enquadramento do projeto

O SaborGest é uma aplicação destinada a pequenas padarias, pastelarias e estabelecimentos semelhantes, com o objetivo de facilitar a gestão de colaboradores, turnos, assiduidade e stock.

Os principais utilizadores são o gerente, responsável pela gestão do estabelecimento, e os funcionários, que utilizam a aplicação para registar a sua atividade e consultar informação pessoal.

Entre as funcionalidades encontram-se a gestão de colaboradores, criação e atribuição de turnos, registo de entrada e saída, cálculo de horas trabalhadas, gestão de ausências e controlo de stock.

O projeto utiliza uma aplicação Web, destinada ao gerente, e uma aplicação Android, destinada aos funcionários. O desenvolvimento decorre ao longo do semestre letivo. A 20/11/2026 foi apresentado ao docente o estado atual da aplicação, através de uma demonstração direta das funcionalidades já desenvolvidas na aplicação Web e Android.

Até ao momento, ainda não foi possível estabelecer contacto com um responsável real de uma padaria ou pastelaria. O docente acompanha o projeto, mas não existe disponibilidade semanal de um cliente externo confirmada.

### B1. Escolha de Kanban

Escolheria o Kanban como abordagem principal para organizar o desenvolvimento do SaborGest.

Esta escolha justifica-se por duas características do projeto:

- O SaborGest está dividido em diferentes componentes, como a aplicação Web, a aplicação Android e a API, permitindo que várias tarefas sejam desenvolvidas em simultâneo.
- As prioridades podem ser ajustadas durante o desenvolvimento, uma vez que novas funcionalidades e melhorias vão sendo identificadas à medida que o projeto evolui.

Uma vantagem do Kanban é permitir acompanhar facilmente o estado das tarefas e identificar o trabalho que está bloqueado ou atrasado.

Uma dificuldade poderá ser coordenar os diferentes elementos do grupo e garantir que as tarefas desenvolvidas em separado funcionam corretamente quando são integradas.

### B2. Itens de trabalho e primeira entrega

Para organizar o desenvolvimento do SaborGest, proporia a seguinte ordem de prioridades:

1. **Gestão de colaboradores e turnos:** permitir ao gerente registar colaboradores, criar turnos e associá-los aos funcionários.
2. **Registo de entrada e saída:** permitir aos funcionários registar o início e o fim do turno, apenas quando existe uma atribuição prévia por parte do gerente.
3. **Cálculo e consulta de horas:** calcular automaticamente as horas trabalhadas e permitir ao gerente consultar os resultados.
4. **Gestão de stock:** permitir registar e consultar movimentos de stock dos produtos do estabelecimento.

**Primeira entrega**

Incluiria os três primeiros itens, porque representam as funcionalidades principais do SaborGest e permitem gerir os turnos e acompanhar as horas trabalhadas pelos funcionários.

A gestão de stock seria considerada uma entrega complementar. O módulo já tem desenvolvimento realizado, pelo que o trabalho nesta fase passaria por continuar a sua validação e integração com o restante sistema.

**Critério de aceitação - Registo de entrada e saída**

Um funcionário com um turno previamente atribuído pelo gerente deve conseguir registar a entrada e a saída. Um funcionário sem um turno atribuído não deve conseguir efetuar esses registos.

**Teste de verificação**

Criar dois funcionários de teste, atribuindo um turno apenas a um deles. Tentar realizar os registos de entrada e saída com ambos. O teste será considerado aprovado se apenas o funcionário com turno atribuído conseguir efetuar os registos e se os horários ficarem associados ao funcionário e ao turno corretos.

### B3. Práticas de XP e bloqueio no Kanban

**Prática 1 - Programação a pares**

Dois elementos do grupo poderiam trabalhar em conjunto numa funcionalidade, por exemplo, no registo de entrada e saída dos funcionários. Enquanto um elemento escreve o código, o outro acompanha o desenvolvimento, verifica as regras de funcionamento e ajuda a identificar possíveis erros. Os elementos podem trocar de funções durante o trabalho.

**Prática 2 - Desenvolvimento orientado a testes (TDD)**

Antes de implementar uma funcionalidade, a equipa poderia criar testes para verificar o comportamento esperado. Por exemplo, no registo de assiduidade, seria criado primeiro um teste para confirmar que um funcionário sem turno atribuído não consegue registar a entrada. Depois seria desenvolvido o código necessário para o teste passar e, por fim, melhorada a estrutura do código, mantendo o resultado esperado.

**Situação de bloqueio no Kanban**

Considerando que existem dois itens em curso numa etapa cujo limite WIP é dois, a equipa já atingiu o número máximo de tarefas permitido nessa etapa.

Se um teste estiver bloqueado por falta de acesso ao ambiente, a equipa deverá assinalar esse bloqueio no quadro e procurar resolver o problema, por exemplo, solicitando as permissões necessárias ou pedindo apoio ao responsável pelo ambiente.

Enquanto o problema não estiver resolvido, os elementos devem colaborar para desbloquear o teste e avançar com as tarefas que já estão em curso. Não devem iniciar um novo item nessa etapa, porque isso ultrapassaria o limite WIP definido.

O objetivo é terminar ou desbloquear o trabalho existente antes de começar novas tarefas, evitando acumular trabalho por concluir.