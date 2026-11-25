# Atividade 07 - Princípios AGILE

## Parte A - Compreensão dos conceitos

### 1. Desenvolvimento ágil e relação entre Agile e Scrum

O desenvolvimento ágil é uma forma de desenvolver software através de etapas mais curtas, permitindo testar funcionalidades, receber opiniões e fazer alterações ao longo do projeto. O objetivo é conseguir adaptar o desenvolvimento às necessidades dos utilizadores, sem ter de esperar pelo produto completo.

O Agile representa um conjunto de valores e princípios, enquanto o Scrum é uma metodologia de trabalho, mais propriamente uma framework, que permite aplicar esses princípios na organização de uma equipa.

### 2. Os quatro valores do Manifesto Ágil

Os quatro valores do Manifesto Ágil dão mais importância a:

- Pessoas e comunicação dentro da equipa do que apenas processos e ferramentas.
- Ter software funcional do que produzir muita documentação.
- Trabalhar em conjunto com o cliente do que estar focado apenas em contratos.
- Conseguir adaptar-se a mudanças do que seguir sempre o plano inicial.

Isto não significa que o planeamento e a documentação deixem de ser importantes. Continuam a ser necessários para organizar o trabalho e manter a informação, mas não devem impedir a equipa de comunicar e adaptar-se quando é preciso.

### 3. Desenvolvimento iterativo e incremental

O desenvolvimento iterativo consiste em voltar a trabalhar numa funcionalidade que já existe, procurando corrigir problemas ou melhorar o seu funcionamento.

O desenvolvimento incremental consiste em acrescentar novas funcionalidades à aplicação, aumentando progressivamente aquilo que o sistema consegue fazer.

Por exemplo, no SaborGest, melhorar o registo de assiduidade depois de realizar testes seria uma iteração. Acrescentar o módulo de gestão de stock seria um incremento.

### 4. Colaboração com o cliente e retorno frequente

A colaboração com o cliente é importante porque permite perceber melhor aquilo de que realmente precisa e evitar desenvolver funcionalidades que não correspondem às suas necessidades. Ao apresentar versões do software com frequência, a equipa consegue receber opiniões e corrigir problemas mais cedo.

Isto está relacionado com o princípio de trabalhar regularmente com o cliente e com o princípio de entregar software funcional frequentemente, permitindo melhorar o produto ao longo do desenvolvimento.

### 5. Reação a um novo requisito

Quando surge um novo requisito, a equipa deve primeiro perceber o que é pretendido, avaliar a sua importância e analisar o impacto que terá no projeto.

Depois, deve decidir se faz sentido alterar as prioridades e quando implementar essa funcionalidade. Aceitar mudanças não significa fazer tudo imediatamente, porque existem prazos, recursos e outras tarefas importantes que também precisam de ser concluídas.

### 6. Ritmo sustentável e simplicidade

O ritmo sustentável significa que a equipa deve conseguir trabalhar de forma regular, sem estar constantemente sobrecarregada ou depender de horas excessivas de trabalho para cumprir os objetivos. Uma prática seria organizar tarefas de acordo com o tempo e a disponibilidade dos elementos.

A simplicidade consiste em desenvolver apenas aquilo que é necessário, evitando funcionalidades ou complexidade que não acrescentam valor ao projeto. Uma prática seria começar por implementar as funcionalidades essenciais e deixar as restantes para fases posteriores.

### 7. Qualidade técnica e agilidade

A qualidade técnica é importante para o desenvolvimento ágil porque permite fazer alterações e acrescentar funcionalidades sem provocar constantemente novos problemas no sistema.

Duas práticas que ajudam a manter essa qualidade são a realização de testes ao código desenvolvido e a revisão do código antes de integrar alterações no projeto. Desta forma, é mais fácil detetar erros e manter o sistema organizado.

### 8. Auto-organização e reflexão sobre a forma de trabalhar

A auto-organização significa que a própria equipa consegue organizar o trabalho, dividir tarefas e decidir como atingir os objetivos definidos, sem depender constantemente de alguém para indicar todos os passos.

A reflexão sobre a forma de trabalhar consiste em analisar regularmente o que correu bem e o que poderia ser melhorado. Ambas são importantes porque permitem que a equipa trabalhe com mais autonomia, identifique problemas e melhore a sua organização ao longo do projeto.

## Parte B - Aplicação ao projeto de PdS (SaborGest)

### Enquadramento do projeto

O SaborGest é uma aplicação destinada a pequenas padarias, pastelarias e estabelecimentos semelhantes, com o objetivo de facilitar a gestão de colaboradores, turnos, assiduidade e stock.

Os principais utilizadores são o gerente, que gere o estabelecimento e consulta a informação, e os funcionários, que utilizam a aplicação para registar a sua atividade.

Entre as funcionalidades desenvolvidas encontram-se a gestão de colaboradores e turnos, o registo de entrada e saída, o cálculo de horas trabalhadas, a gestão de ausências e o controlo de stock.

O desenvolvimento está dividido entre uma aplicação Web, destinada ao gerente, e uma aplicação Android, destinada aos funcionários.

O projeto está a ser desenvolvido ao longo do semestre, no âmbito da unidade curricular. Ainda não foi possível estabelecer contacto com um responsável real de uma padaria ou pastelaria, pelo que não existe disponibilidade de um cliente externo confirmada. O docente acompanha o projeto e o grupo pode avaliar internamente as versões desenvolvidas.

### B1. Abordagem de desenvolvimento

Escolheria uma abordagem predominantemente ágil, porque o SaborGest tem sido desenvolvido por módulos e as funcionalidades têm sido acrescentadas e ajustadas ao longo do projeto. Além disso, são realizados testes durante o desenvolvimento, permitindo identificar problemas e melhorar o que já foi implementado.

Esta abordagem também permite adaptar as prioridades quando surgem novas necessidades. No entanto, como ainda não foi possível obter feedback de utilizadores reais, será importante tentar envolver potenciais utilizadores numa fase posterior.

### B2. Primeira e segunda entregas

**Primeira entrega**

A primeira versão útil do SaborGest deverá permitir ao gerente registar colaboradores, criar turnos e associá-los aos funcionários. Os funcionários deverão conseguir registar a entrada e a saída dos turnos que lhes foram previamente atribuídos. O gerente deverá conseguir consultar as horas trabalhadas.

**Segunda entrega**

Numa segunda versão, poderão ser acrescentadas funcionalidades de gestão de ausências, pedidos de troca de turnos e controlo de stock, complementando as funcionalidades principais.

Caso, depois da primeira demonstração, o cliente pedisse prioridade para o cancelamento de pedidos de troca de turno, reorganizaria esta segunda entrega para incluir essa funcionalidade mais cedo. As estatísticas e os relatórios mais detalhados ficariam adiados para uma versão posterior, dando prioridade ao que o cliente considera mais importante.

Desta forma, o desenvolvimento seria ajustado com base no feedback recebido, sem ser necessário alterar todo o trabalho já realizado.

### B3. Princípios Agile aplicados ao SaborGest

**Princípio 1 - Entregar software funcional com frequência**

A equipa deve desenvolver e testar as funcionalidades por etapas, procurando ter versões funcionais que permitam verificar o progresso do SaborGest, em vez de deixar todos os testes para o final.

**Princípio 2 - Aceitar alterações aos requisitos**

Quando surgirem novas necessidades ou alterações, a equipa deverá avaliar a sua importância e ajustar as prioridades. Por exemplo, se for necessário acrescentar o cancelamento de pedidos de troca de turno, essa funcionalidade poderá passar a ter prioridade sobre outras menos importantes.

**Princípio 3 - Manter uma boa qualidade técnica**

A equipa deverá realizar testes regularmente, rever o código e verificar se as alterações realizadas não provocam problemas noutras partes da aplicação. Isto é especialmente importante porque o SaborGest utiliza uma aplicação Web, uma aplicação Android, uma API e uma base de dados que precisam de funcionar em conjunto.

**Funcionalidade escolhida para validação: Registo de entrada e saída dos funcionários**

O objetivo é confirmar que apenas os funcionários com um turno previamente atribuído pelo gerente conseguem registar a entrada e a saída.

**Critério de aceitação**

- Um funcionário com um turno previamente atribuído deve conseguir registar a entrada e a saída.
- Um funcionário sem um turno atribuído não deve conseguir efetuar esses registos.
- Os horários registados devem ficar associados ao funcionário e ao respetivo turno.

**Teste proposto**

Criar dois funcionários de teste, atribuindo um turno apenas a um deles. Depois, tentar efetuar os registos de entrada e saída com ambos. O teste será considerado aprovado se o funcionário com turno conseguir realizar os registos e o funcionário sem turno receber uma indicação de que não tem um turno atribuído.