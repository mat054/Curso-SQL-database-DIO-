# Curso-SQL-database-DIO-

Mudanças:
1. Adicionei o atributo "solicitar cancelamento" (boolean) na entidade Pedido
2. Coloquei Pessoa física e Pessoa jurídica herdando de cliente
3. Adicionei a entidade pagamento que possui como atributos (id, forma de pagamento, status do pagamento, data e hora do pagamento e valor)

Pagamento se relaciona de 1:n com cliente, pois cliente pode ter vários pagamento (pode estar pagando vários pedidos ao mesmo tempo) enquanto cada pagamento só tem um cliente específico

Pagamento se relaciona de 1:n com pedido, pois cada pagamento só tem um pedido, mas cada pedido pode ter mais de um pagamento, como no caso do parcelamento, que são feitos vários pagamentos para um mesmo pedido

4. Adicionei a entidade entrega, que possui como atributos (id da entrega, endereço da entrega, data prevista para a entrega, data da entrega (quando o produto efetivamente chega no destinatário), status da entrega e código de rastreamento)

Entrega se relaciona com pedido de 1:1, pois cada entrega está relacionado a um único pedido (considerando que a entrega seja feita com todos os produtos do pedido juntos), e cada pedido à uma única entrega

E entrega se relaciona com cliente de 1:n, pois cada entrega está relacionado a um único cliente, mas um cliente pode ter vários pedidos e consequentemente várias entregas para ele.
