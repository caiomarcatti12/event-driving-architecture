## **Introdução ao Event-Driven**
A arquitetura orientada a eventos, conhecida como **Event-Driven Architecture (EDA)**, é um estilo de design de software que depende da geração, detecção, consumo e reação a eventos. Um **evento** é uma mudança de estado ou uma atualização em um sistema, como um pedido criado, um pagamento processado ou um usuário registrado.

Na EDA, os componentes do sistema atuam de forma independente e se comunicam reagindo a esses eventos, em vez de utilizar chamadas síncronas diretas. Essa abordagem traz inúmeros benefícios, como:

1. **Desacoplamento**: Os serviços ou componentes são independentes e podem evoluir sem impactar outros diretamente. Isso facilita a escalabilidade e a manutenção.
2. **Escalabilidade e Resiliência**: Com a EDA, cada componente pode ser escalado de forma independente, tornando o sistema mais resiliente a falhas. Se um componente falhar, os outros continuam a funcionar.
3. **Reatividade**: O sistema pode responder de forma imediata a mudanças, permitindo uma experiência mais dinâmica e responsiva para o usuário.

**Exemplo Simplificado**: Imagine um sistema de e-commerce. Quando um cliente faz um pedido, um evento de "pedido criado" é gerado. Diversos serviços, como pagamento, estoque e entrega, podem reagir a esse evento, processando cada etapa do pedido de forma independente.

A arquitetura event-driven se destaca especialmente em sistemas distribuídos, onde diferentes serviços precisam colaborar de forma assíncrona para executar tarefas complexas.
