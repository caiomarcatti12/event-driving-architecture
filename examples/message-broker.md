# Uso do event driving com mensageria

A programação orientada a eventos pode ser usada com sistemas de middleware orientado a mensagens (MOM), como agentes de mensagens.

Em um sistema orientado a mensagens, os eventos são normalmente representados como mensagens enviadas entre diferentes componentes ou sistemas. Quando um componente recebe uma mensagem, ele pode acionar uma resposta orientada a eventos.

Por exemplo, considere um sistema que consiste em um intermediário de mensagens e dois componentes: um produtor e um consumidor. O produtor envia mensagens ao intermediário e o consumidor recebe mensagens do intermediário.

O consumidor pode ser implementado como um aplicativo orientado a eventos que aguarda a chegada das mensagens e as processa assim que chegam. Isso permite que o consumidor responda às mensagens assim que chegam, em vez de ter que pesquisar novas mensagens no intermediário .

No geral, a programação orientada a eventos é um ajuste natural para sistemas orientados a mensagens porque permite que diferentes componentes se comuniquem por meio da troca de mensagens.


## Exemplo de fluxo
```
+------------+
|  Producer  |
+------------+
      |
      | send message
      v
+------------+
|  Message   |
|   Broker   |
+------------+
      |
      | receive message
      v
+------------+
|  Consumer  |
+------------+
```

Neste exemplo, o produtor envia uma mensagem para o message broker, que então encaminha a mensagem para o consumidor. 

O consumidor é implementado como um aplicativo orientado a eventos que espera a chegada de mensagens e as processa à medida que chegam.

Este é um exemplo de sistema orientado a eventos porque o fluxo do programa é determinado por eventos (a chegada de mensagens) em vez de ser predeterminado pelo próprio programa.

Eu espero que isso ajude! Deixe-me saber se você tem alguma dúvida.