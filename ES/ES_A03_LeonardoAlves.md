# Atividade 03 - Produto Request

## 1. Identificação e problema a resolver

Em pequenas padarias e pastelarias, o controlo de turnos e de horas de trabalho é frequentemente feito de forma manual, em papel ou em folhas de cálculo dispersas, ou recorrendo a aplicações genéricas não pensadas para este tipo de negócio. Isto dificulta saber, a qualquer momento, quem está a trabalhar, quantas horas cada colaborador já cumpriu, e se houve lugar a horas extra.

O principal objetivo da aplicação é automatizar o registo de entrada e saída dos colaboradores e o cálculo das respetivas horas, reduzindo o esforço manual do gerente e o risco de erro no cálculo de horas extra.

Dúvida a esclarecer: não temos ainda uma noção concreta e confirmada do impacto real destes problemas (por exemplo, quanto tempo um gerente perde tipicamente com este cálculo, ou com que frequência ocorrem erros). Esta informação seria idealmente obtida junto de um responsável real de um negócio deste tipo.

## 2. Utilizadores e pessoas a consultar

Foram identificados dois perfis de utilizador:

- **Gerente:** pretende planear turnos, gerir colaboradores e ter visibilidade sobre as horas trabalhadas e horas extra, sem ter de as calcular manualmente.
- **Funcionário:** pretende registar de forma simples o início e o fim do seu turno, e consultar o seu próprio histórico de horas.

Pessoas identificadas que poderão esclarecer necessidades:

- O docente responsável pelo PDS, que propôs e acompanha o projeto, pode esclarecer o âmbito esperado e restrições técnicas.
- Um responsável real de uma padaria ou pastelaria, ainda não foi possível estabelecer contacto. A referência usada até agora (uma padaria em Coimbra, mencionada como inspiração inicial) serve apenas de contexto e não corresponde a dados reais recolhidos nem a uma validação efetiva das necessidades.

## 3. Recolha inicial de informação

Perguntas preparadas para um futuro responsável de padaria/pastelaria:

- Como é feito hoje o registo de turnos e de horas trabalhadas?
- Como são calculadas atualmente as horas extra, quando existem?
- Que informação é indispensável constar num resumo de horas de um colaborador?
- Existem regras específicas (por exemplo, intervalos obrigatórios) que o sistema deve respeitar?
- Quantos colaboradores tem tipicamente um negócio deste género, e quantos turnos diferentes costumam existir por dia?

**Estado da recolha**

Até ao momento, não foram realizadas entrevistas nem recolhidos dados diretamente junto de responsáveis ou funcionários de padarias e pastelarias. As necessidades identificadas resultam da análise inicial do problema e das ideias discutidas pelo grupo durante a conceção do projeto.

As respostas às perguntas preparadas encontram-se, por isso, pendentes de validação junto de potenciais utilizadores. O docente responsável pelo PDS poderá também esclarecer questões relacionadas com o âmbito e os requisitos académicos do projeto.

## 4. Funcionalidades inicialmente identificadas

Com base na análise inicial do problema e nas necessidades identificadas pelo grupo, foram propostas as seguintes funcionalidades para a aplicação:

| Código | Funcionalidade | Descrição |
|---|---|---|
| R01 | Gestão de colaboradores | O sistema deve permitir ao gerente registar, consultar, editar e gerir os colaboradores. |
| R02 | Gestão de turnos | O sistema deve permitir ao gerente criar, consultar, editar e organizar os turnos de trabalho. |
| R03 | Atribuição de turnos | O sistema deve permitir ao gerente associar colaboradores aos respetivos turnos. |
| R04 | Registo de entrada | O sistema deve permitir ao funcionário registar o início do seu turno, desde que tenha um turno previamente atribuído pelo gerente. |
| R05 | Registo de saída | O sistema deve permitir ao funcionário registar o fim do turno que lhe foi previamente atribuído. |
| R06 | Cálculo de horas trabalhadas | O sistema deve calcular automaticamente o total de horas trabalhadas por cada colaborador, com base nos registos de entrada e saída. |
| R07 | Consulta de horas trabalhadas | O sistema deve permitir ao gerente consultar as horas trabalhadas pelos colaboradores. |
| R08 | Cálculo de horas extraordinárias | O sistema deve identificar e calcular as horas extraordinárias realizadas pelos colaboradores, de acordo com as regras definidas. |
| R09 | Histórico individual de horas | O sistema deve permitir ao funcionário consultar o seu próprio histórico de horas trabalhadas. |
| R10 | Resumo de horas por colaborador | O sistema deve permitir ao gerente consultar um resumo das horas trabalhadas e extraordinárias de cada colaborador. |

## 5. Prioridades e condições já conhecidas

**Prioridades das funcionalidades**

Para uma primeira versão da aplicação, foram consideradas essenciais as funcionalidades relacionadas com a gestão de colaboradores e turnos, o registo de entrada e saída e o cálculo das horas trabalhadas e extraordinárias.

Assim, as prioridades inicialmente definidas são:

- **Essenciais (R01 a R08):** gestão de colaboradores, criação e atribuição de turnos, registo de entrada e saída, cálculo de horas trabalhadas e extraordinárias e consulta das horas pelo gerente.
- **Secundárias (R09 e R10):** consulta do histórico individual pelo funcionário e consulta de um resumo detalhado das horas por colaborador.

Esta divisão representa uma proposta inicial do grupo e poderá ser ajustada após a validação das necessidades junto de potenciais utilizadores.

**Condições já conhecidas**

- **Aplicação Web:** destinada ao gerente, permitindo gerir colaboradores, organizar turnos e consultar as horas trabalhadas.
- **Aplicação Android:** destinada aos funcionários, permitindo registar a entrada e saída dos turnos e consultar o seu histórico.
- **Perfis de utilizador:** a aplicação deverá distinguir, pelo menos, dois perfis: gerente e funcionário, com diferentes permissões e funcionalidades.
- **Atribuição prévia de turnos:** o funcionário só poderá registar a entrada e a saída quando tiver um turno previamente atribuído pelo gerente.

Estas condições resultam das decisões iniciais do grupo durante a conceção do projeto. A necessidade de ligação à Internet e a possibilidade de funcionamento sem ligação ainda não foram definidas.

## 6. Dúvidas e próximos passos

Apesar de já terem sido identificadas algumas necessidades e funcionalidades, existem questões que ainda precisam de ser esclarecidas antes de avançar para uma definição mais completa dos requisitos.

**Questões por esclarecer**

- Como são organizados atualmente os turnos numa padaria ou pastelaria? A esclarecer junto de um responsável de um negócio deste género.
- Que regras devem ser aplicadas ao cálculo das horas extraordinárias? A esclarecer junto de um responsável e, se necessário, através de pesquisa sobre as regras aplicáveis.
- Existem intervalos de descanso obrigatórios que devem ser considerados no cálculo das horas trabalhadas? A esclarecer junto de um responsável e através da análise das regras aplicáveis.
- Que informação deve estar disponível no histórico individual dos funcionários? A esclarecer junto de potenciais funcionários e do gerente.
- A aplicação necessita de funcionar sem ligação à Internet? A definir pelo grupo, considerando as condições reais de utilização.
- As prioridades e funcionalidades inicialmente propostas correspondem às necessidades reais dos utilizadores? A validar através de entrevistas com um responsável e potenciais funcionários de uma padaria ou pastelaria.

**Próximos passos**

Como próximos passos, pretende-se contactar um responsável de uma padaria ou pastelaria e, se possível, alguns funcionários, de forma a recolher informação sobre os métodos de trabalho utilizados atualmente.

Depois dessa recolha, será possível confirmar ou ajustar as funcionalidades identificadas, esclarecer as regras de negócio e rever as prioridades definidas pelo grupo.

O objetivo é garantir que a aplicação responde efetivamente aos problemas identificados e às necessidades dos seus futuros utilizadores.