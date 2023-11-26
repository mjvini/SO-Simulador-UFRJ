# Objetivo do Trabalho

Estimular a capacidade do aluno de trabalhar em equipe para organizar, projetar e desenvolver
soluções para problemas formulados que envolvam o estudo e o conhecimento sobre
gerenciamentos do sistema operacional.

# Escopo do Trabalho
- Desenvolver um simulador que implementa o algoritmo de escalonamento de processos, usando
a estratégia de seleção Round Robin (ou Circular) com Feedback.
- Preparar um relatório contendo uma descrição sobre os objetivos do trabalho, as premissas
consideradas no desenvolvimento do escalonador e a saída da execução do simulador.
-  Os trabalhos devem ser feitos exclusivamente em C.
- As avaliações sobre o funcionamento dos simuladores serão feitas em horário marcado.

# Premissas a serem definidas pelo grupo para o desenvolvimento do simulador
- Limite máximo de processos criados;
- O valor da fatia de tempo dada aos processos em execução;
- Tempos de serviço e de I/O aleatórios para cada processo criado;
- Tempos de duração de cada tipo de I/O (disco, fita magnética e impressora);
- Gerência de Processos
  - Definição do PID de cada processo,
  - Informações do PCB (contexto de software – prioridade, PID, PPID, status);
  - Escalonador (pelo menos 3 filas, sendo uma fila de alta e uma de baixa prioridade
para execução na CPU, e 1 fila de I/O, que pode ser implementada com filas
diferentes para cada tipo de dispositivo);
- Tipos de I/O
  - Disco – retorna para a fila de baixa prioridade;
  - Fita magnética - retorna para a fila de alta prioridade;
  - Impressora - retorna para a fila de alta prioridade;
- Ordem de entrada na fila de prontos
  - Processos novos - entram na fila de alta prioridade;
  - Processos que retornam de I/O – dependente do tipo de I/O solicitado;
  - Processos que sofreram preempção – retornam na fila de baixa prioridade.

