## Deadlock

Deadlock é quando um ou mais processos ficam impedidos de executar, esses processos podem estar competindo recursos entre eles (cpu, memória, dados, etc), criando assim loopings infinitos e awaits sem retorno. 
Esses processos ficam presos e ficam utilizando um alto índice de CPU, que pode causar perda de performance e exceptions nos sistemas.
Um exemplo de Deadlock em Java, seria o uso de `synchronized methods` que ficam dependendo um do outro, assim entrando em looping.
Outro exemplo seria diversos processos tentando acessar uma tabela de um banco de dados relacional ao mesmo tempo, esses processos podem entrar em conflitos.


### Formas de resolver ou evitar deadlocks.

- Identificar o processo que está preso a muito tempo e matar esse processo de menos importância.
- Organizar processos em uma fila (`RabbitMQ`, `0MQ`) e consumir essa fila de forma que seja executado cada `message` na sua vez, evitando conflitos.
- Imutabilidade de objetos, você pode ler os objetos imutáveis livremente, sem se preocupar se o estado desse objeto vai ser alterado, isso permite gerenciar a concorrência de forma mais eficiente.
