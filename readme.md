# O que é o event driving 

A programação orientada a eventos é um paradigma de programação no qual o fluxo do programa é determinado por eventos como ações do usuário, saídas de sensores ou mensagens de outros programas ou threads. Na programação orientada a eventos, um trecho de código é escrito para especificar o que deve acontecer quando um determinado evento ocorrer. O programa então espera que os eventos ocorram e, quando ocorre, executa o código apropriado.

Uma das principais vantagens da programação orientada a eventos é que ela permite que o programa responda aos eventos à medida que eles acontecem, em vez de ter que pesquisar eventos constantemente. Isso pode tornar o programa mais eficiente e responsivo.

A programação orientada a eventos é comumente usada na programação de interface gráfica do usuário (GUI), programação de rede e outras situações em que um programa precisa responder a eventos externos. Também é frequentemente usado em arquiteturas orientadas a eventos, onde diferentes componentes de um sistema se comunicam entre si por meio de eventos.

# Vantagens de se usar essa arquitetura
Existem várias vantagens em usar a programação orientada a eventos:

- Capacidade de resposta: como o programa está aguardando a ocorrência de eventos em vez de pesquisá-los constantemente, ele pode responder a eventos assim que eles ocorrem, tornando-o mais responsivo à entrada do usuário ou a outros eventos externos.

- Eficiência: Os programas orientados a eventos geralmente são mais eficientes porque não desperdiçam recursos pesquisando constantemente eventos que podem não ocorrer.

- Modularidade: os programas orientados a eventos podem ser mais fáceis de modificar e manter, porque geralmente são divididos em unidades menores e independentes que são acionadas por eventos.


# Desvantagens
No entanto, também existem algumas desvantagens potenciais no uso da programação orientada a eventos:

- Complexidade: Os programas orientados a eventos podem ser mais complexos de projetar e implementar, especialmente se houver muitos eventos diferentes que precisam ser manipulados.

- Depuração: A depuração de programas orientados a eventos pode ser mais difícil porque pode ser difícil reproduzir a sequência de eventos que levaram a um bug.

- Teste: Testar programas orientados a eventos pode ser mais desafiador porque pode ser difícil prever a sequência exata de eventos que ocorrerão durante o teste.

No geral, a programação orientada a eventos pode ser uma ferramenta útil para criar programas responsivos e eficientes, mas é importante considerar cuidadosamente as compensações ao decidir se deve usá-la.

# Quando usar

A programação orientada a eventos é adequada para situações em que um programa precisa responder a eventos externos em tempo real. Alguns exemplos comuns incluem:

- Interfaces gráficas do usuário (GUIs): A programação orientada a eventos é frequentemente usada para criar aplicativos GUI porque permite que o programa responda à entrada do usuário (como cliques do mouse e pressionamentos de tecla) conforme ela ocorre.

- Programação de rede: A programação orientada a eventos é frequentemente usada na programação de rede porque permite que o programa responda a solicitações ou dados de entrada de rede à medida que chegam, em vez de ter que pesquisá-los constantemente.

- Sistemas de tempo real: A programação orientada a eventos é frequentemente usada em sistemas de tempo real porque permite que o programa responda a eventos conforme eles acontecem, em vez de ter que esperar por um intervalo de pesquisa regular.

- Sistemas embarcados: A programação orientada a eventos é frequentemente usada em sistemas embarcados porque permite que o programa responda a eventos de sensores ou outros dispositivos externos conforme eles ocorrem.

No geral, a programação orientada a eventos é uma boa escolha sempre que você precisar que um programa responda a eventos externos em tempo real. Não é necessariamente a melhor escolha para todos os tipos de programas, mas pode ser uma ferramenta poderosa no contexto certo.

# Boas práticas
Aqui estão algumas práticas recomendadas para implementar sistemas orientados a eventos:

- Desacoplar componentes: é importante projetar sistemas orientados a eventos de forma que os componentes sejam desacoplados uns dos outros. Isso significa que os componentes não devem ter dependências diretas entre si, mas devem se comunicar por meio de eventos ou mensagens. Isso facilita a modificação ou substituição de componentes sem afetar o restante do sistema.

- Use comunicação assíncrona: a comunicação assíncrona pode ajudar a melhorar o desempenho e a escalabilidade de sistemas orientados a eventos. Isso significa que os componentes não devem bloquear enquanto aguardam uma resposta de outros componentes, mas devem continuar processando e ser notificados quando uma resposta estiver disponível.

- Trate os erros de maneira elegante: é importante lidar com os erros de maneira adequada em sistemas orientados a eventos. Isso pode envolver a repetição de eventos com falha, registro de erros ou envio de notificações para alertar as partes apropriadas.

- Use estruturas de dados apropriadas: As estruturas de dados usadas em um sistema orientado a eventos devem ser escolhidas com base nos requisitos do sistema. Por exemplo, se o sistema precisa suportar grandes volumes de eventos, pode ser necessária uma estrutura de dados otimizada para alto desempenho e escalabilidade.

- Use formatos de mensagem apropriados: Os formatos de mensagem usados ​​em um sistema orientado a eventos devem ser escolhidos com base nos requisitos do sistema. Por exemplo, se o sistema precisar suportar a troca de estruturas de dados complexas, pode ser necessário um formato de mensagem que seja capaz de representar essas estruturas (como JSON ou XML).

No geral, é importante considerar cuidadosamente o design e a implementação de sistemas orientados a eventos para garantir que sejam confiáveis, escaláveis ​​e de fácil manutenção.

# Considerações finais

Aqui estão algumas considerações a ter em mente ao implementar sistemas orientados a eventos:

- Desempenho e escalabilidade: os sistemas orientados a eventos podem lidar com grandes volumes de eventos, mas é importante projetá-los tendo em mente o desempenho e a escalabilidade. Isso pode envolver o uso de estruturas de dados e formatos de mensagens eficientes, bem como a otimização do processamento de eventos.

- Manipulação de erros: é importante lidar com erros normalmente em sistemas orientados a eventos. Isso pode envolver a repetição de eventos com falha, registro de erros ou envio de notificações para alertar as partes apropriadas.

- Simultaneidade: os sistemas orientados a eventos geralmente envolvem vários encadeamentos ou processos em execução simultaneamente. É importante considerar como esses threads ou processos irão interagir e garantir que o sistema seja thread-safe.

- Depuração: a depuração de sistemas orientados a eventos pode ser mais desafiadora do que a depuração de programas sequenciais tradicionais porque pode ser difícil reproduzir a sequência de eventos que levou a um bug. É importante usar ferramentas apropriadas de registro e depuração para ajudar a identificar e corrigir erros em sistemas orientados a eventos.

- Teste: Testar sistemas orientados a eventos pode ser mais desafiador do que testar programas sequenciais tradicionais porque pode ser difícil prever a sequência exata de eventos que ocorrerão durante o teste. É importante usar ferramentas e técnicas de teste apropriadas (como testes de unidade, testes de integração e testes de estresse) para garantir que o sistema seja confiável e funcione bem em diferentes condições.

No geral, é importante considerar cuidadosamente o design e a implementação de sistemas orientados a eventos para garantir que sejam confiáveis, escaláveis ​​e de fácil manutenção.


# Exemplos

- [Python](examples/python.md)
- [Mensageria](examples/message-broker.md)
