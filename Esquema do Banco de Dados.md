## Esquema do Banco de Dados

### Controle de Estoque

**Tabela: produtos**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `nome` (TEXT, NOT NULL)
- `tipo` (TEXT, NOT NULL) -- e.g., 'alimento', 'bebida', 'limpeza'
- `quantidade_atual` (INTEGER, NOT NULL, DEFAULT 0)
- `quantidade_minima` (INTEGER, NOT NULL, DEFAULT 0)
- `unidade_medida` (TEXT) -- e.g., 'unidade', 'litro', 'kg'

**Tabela: movimentacoes_estoque**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `produto_id` (INTEGER, NOT NULL, FOREIGN KEY para produtos.id)
- `tipo_movimentacao` (TEXT, NOT NULL) -- 'entrada' ou 'saida'
- `quantidade` (INTEGER, NOT NULL)
- `data_hora` (DATETIME, DEFAULT CURRENT_TIMESTAMP)
- `observacao` (TEXT)




### Controle de Frigobar

**Tabela: itens_frigobar**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `nome` (TEXT, NOT NULL)
- `preco` (REAL, NOT NULL)
- `produto_id` (INTEGER, FOREIGN KEY para produtos.id, NULLABLE) -- Opcional, se o item do frigobar for um produto do estoque geral

**Tabela: frigobares**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `quarto_id` (INTEGER, NOT NULL, UNIQUE, FOREIGN KEY para quartos.id)

**Tabela: frigobar_consumo**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `frigobar_id` (INTEGER, NOT NULL, FOREIGN KEY para frigobares.id)
- `item_frigobar_id` (INTEGER, NOT NULL, FOREIGN KEY para itens_frigobar.id)
- `quantidade` (INTEGER, NOT NULL)
- `data_consumo` (DATETIME, DEFAULT CURRENT_TIMESTAMP)
- `hospede_id` (INTEGER, FOREIGN KEY para hospedes.id, NULLABLE)




### Acompanhamento de Pedidos de Clientes

**Tabela: pedidos**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `hospede_id` (INTEGER, NOT NULL, FOREIGN KEY para hospedes.id)
- `quarto_id` (INTEGER, NOT NULL, FOREIGN KEY para quartos.id)
- `data_hora_pedido` (DATETIME, DEFAULT CURRENT_TIMESTAMP)
- `status` (TEXT, NOT NULL) -- e.g., 'pendente', 'em preparo', 'entregue', 'cancelado'
- `observacoes` (TEXT)

**Tabela: itens_pedido**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `pedido_id` (INTEGER, NOT NULL, FOREIGN KEY para pedidos.id)
- `produto_id` (INTEGER, FOREIGN KEY para produtos.id, NULLABLE) -- Se for um item do estoque geral
- `nome_item` (TEXT, NOT NULL) -- Nome do item, caso não seja um produto do estoque
- `quantidade` (INTEGER, NOT NULL)
- `preco_unitario` (REAL, NOT NULL)




### Sistema de Reservas

**Tabela: quartos**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `numero` (TEXT, NOT NULL, UNIQUE)
- `tipo` (TEXT, NOT NULL) -- e.g., 'casal', 'solteiro', 'duplo'
- `capacidade` (INTEGER, NOT NULL)
- `disponivel` (BOOLEAN, NOT NULL, DEFAULT TRUE)

**Tabela: hospedes**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `nome` (TEXT, NOT NULL)
- `sobrenome` (TEXT, NOT NULL)
- `documento` (TEXT, UNIQUE)
- `telefone` (TEXT)
- `email` (TEXT)

**Tabela: reservas**
- `id` (INTEGER, PRIMARY KEY, AUTOINCREMENT)
- `quarto_id` (INTEGER, NOT NULL, FOREIGN KEY para quartos.id)
- `hospede_id` (INTEGER, NOT NULL, FOREIGN KEY para hospedes.id)
- `data_checkin` (DATE, NOT NULL)
- `data_checkout` (DATE, NOT NULL)
- `status_reserva` (TEXT, NOT NULL) -- e.g., 'confirmada', 'cancelada', 'check-in', 'check-out'
- `valor_total` (REAL)


