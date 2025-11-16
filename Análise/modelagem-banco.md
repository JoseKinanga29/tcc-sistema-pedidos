# Modelagem do Banco de Dados

## Tabelas principais

### Usuário
- id (PK)
- nome
- email
- tipo (cliente, administrador)

### Produto
- id (PK)
- nome
- preço
- categoria

### Pedido
- id (PK)
- id_usuario (FK)
- data_hora
- status (pendente, em preparo, pronto)
- total

### Pedido_Produto
- id_pedido (FK)
- id_produto (FK)
- quantidade

## Relacionamentos
- Um usuário pode ter vários pedidos
- Um pedido pode ter vários produtos
