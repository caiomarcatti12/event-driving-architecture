
## **Cenários de Exemplos de Uso**
Aqui estão alguns cenários que ilustram como configurar exchanges e filas no RabbitMQ para diferentes tipos de eventos, com nomes de filas coerentes e prefixados pela exchange para indicar claramente a quem pertencem:

### **Cenário 1: Sistema de E-commerce**
**Descrição**: Quando um pedido é criado, um evento "pedido.criado" é gerado e publicado.
- **Exchange**: `ecommerce.order` (Topic Exchange)
- **Chaves de Roteamento**:
  - `pedido.criado`
  - `pedido.pago`
  - `pedido.cancelado`
- **Filas**:
  - `ecommerce.order.processar-pedido-novo` — Processa eventos de criação de pedidos e inicia o fluxo de processamento.
  - `ecommerce.order.validar-pagamento-pedido` — Verifica se os pagamentos foram concluídos e atualiza o status do pedido.
  - `ecommerce.order.cancelar-pedido` — Processa o cancelamento do pedido, ajustando estoque e notificando o cliente.

### **Cenário 2: Sistema de Monitoramento**
**Descrição**: Quando um serviço está com desempenho abaixo do esperado, ele emite um evento para sinalizar um alerta.
- **Exchange**: `monitoramento.alertas` (Topic Exchange)
- **Chaves de Roteamento**:
  - `alerta.cpu.alto`
  - `alerta.memoria.baixa`
- **Filas**:
  - `monitoramento.alertas.notificar-alerta-cpu` — Envia notificações sobre alto uso de CPU para os responsáveis.
  - `monitoramento.alertas.escalar-alerta-memoria` — Escala recursos automaticamente quando a memória está baixa.

### **Cenário 3: Sistema de Notificações**
**Descrição**: Enviar notificações via e-mail e SMS para usuários.
- **Exchange**: `notificacao.usuario` (Fanout Exchange)
- **Filas**:
  - `notificacao.usuario.enviar-email` — Consumidor que envia e-mails para usuários.
  - `notificacao.usuario.enviar-sms` — Consumidor que envia SMS para usuários.

  