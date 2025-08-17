# Sistema de Gestão para Pousada - Versão Atualizada

## Visão Geral

Este é um sistema completo de gestão para pousadas com 40 quartos, desenvolvido com Flask (backend) e React (frontend). O sistema oferece controle total sobre estoque, frigobar, pedidos de clientes, reservas, **quartos ocupados** e **gestão financeira**.

## Funcionalidades Principais

### 1. Dashboard
- Visão geral da ocupação dos quartos
- Alertas de estoque baixo
- Pedidos pendentes
- Consumo do frigobar
- Atividades recentes do sistema

### 2. **Quartos Ocupados** ⭐ **NOVA FUNCIONALIDADE**
- Visualização de todos os quartos atualmente ocupados
- Detalhes completos do hóspede (nome, documento, contato)
- Período de estadia (check-in, check-out, dias restantes)
- Status de pedidos ativos por quarto
- Histórico completo de pedidos do hóspede
- Valor total da estadia (hospedagem + pedidos)
- Modal detalhado com estatísticas financeiras

### 3. Controle de Estoque
- Cadastro de produtos (alimentos, bebidas, produtos de limpeza)
- Controle de entrada e saída de produtos
- Alertas automáticos para estoque baixo
- Relatórios de movimentação
- Categorização por tipo de produto

### 4. Sistema de Frigobar
- Cadastro de itens do frigobar com preços
- Registro de consumo por quarto
- Controle automático de estoque
- Relatórios de consumo por quarto
- Histórico detalhado de consumo

### 5. Acompanhamento de Pedidos
- Criação de pedidos por quarto/hóspede
- Controle de status (pendente, em preparo, entregue, cancelado)
- Cálculo automático de valores
- Histórico completo de pedidos
- Observações especiais

### 6. Sistema de Reservas
- Cadastro de quartos (solteiro, casal, duplo)
- Gestão de hóspedes
- Controle de disponibilidade
- Check-in e check-out
- Cálculo de diárias
- Relatórios de ocupação

### 7. **Contas a Pagar** ⭐ **NOVA FUNCIONALIDADE**
- Registro de despesas e fornecedores
- Controle de vencimentos e pagamentos
- Alertas para contas vencidas
- Marcação de contas como pagas
- Resumo financeiro (total pendente, pago, vencidas)
- Histórico completo de pagamentos

### 8. **Contas a Receber** ⭐ **NOVA FUNCIONALIDADE**
- Registro de receitas e clientes
- Controle de recebimentos
- Alertas para contas em atraso
- Marcação de contas como recebidas
- Resumo financeiro (total a receber, recebido, em atraso)
- Integração com hospedagens e serviços

## Tecnologias Utilizadas

### Backend
- **Flask**: Framework web Python
- **SQLAlchemy**: ORM para banco de dados
- **SQLite**: Banco de dados
- **Flask-CORS**: Suporte a CORS

### Frontend
- **React**: Biblioteca JavaScript
- **React Router**: Navegação entre páginas
- **Tailwind CSS**: Framework CSS
- **Shadcn/UI**: Componentes de interface
- **Lucide React**: Ícones

## Estrutura do Banco de Dados

### Tabelas Principais
- **produtos**: Controle de estoque geral
- **movimentacoes_estoque**: Histórico de movimentações
- **quartos**: Cadastro de quartos
- **hospedes**: Cadastro de hóspedes
- **reservas**: Controle de reservas
- **itens_frigobar**: Produtos do frigobar
- **frigobar_consumo**: Consumo do frigobar
- **pedidos**: Pedidos dos clientes
- **itens_pedido**: Itens dos pedidos
- **contas_a_pagar**: Controle de despesas ⭐ **NOVA**
- **contas_a_receber**: Controle de receitas ⭐ **NOVA**

## Como Usar o Sistema

### Acesso
O sistema está disponível em: **https://kkh7ikcyvd97.manus.space**

### Navegação
- Use o menu superior para navegar entre as diferentes seções
- Cada seção possui funcionalidades específicas de CRUD (Criar, Ler, Atualizar, Deletar)

### Fluxo de Trabalho Recomendado

1. **Configuração Inicial**
   - Cadastre os 40 quartos da pousada
   - Cadastre os produtos do estoque
   - Configure os itens do frigobar

2. **Operação Diária**
   - Verifique o dashboard para alertas
   - Monitore quartos ocupados e seus pedidos
   - Processe novos pedidos
   - Registre consumo do frigobar
   - Gerencie check-ins e check-outs
   - Controle contas a pagar e receber

3. **Controle Financeiro** ⭐ **NOVO**
   - Registre despesas (fornecedores, contas)
   - Monitore recebimentos de hospedagens
   - Acompanhe vencimentos e atrasos
   - Gere relatórios financeiros

4. **Controle de Estoque**
   - Registre entradas de produtos
   - Monitore alertas de estoque baixo
   - Faça reposições quando necessário

## Características Técnicas

- **Responsivo**: Funciona em desktop e mobile
- **Tempo Real**: Atualizações instantâneas
- **Seguro**: Validações no frontend e backend
- **Escalável**: Arquitetura preparada para crescimento
- **Intuitivo**: Interface amigável e fácil de usar
- **Completo**: Gestão integrada de todas as operações

## Novas Funcionalidades Implementadas

### 🏨 **Quartos Ocupados**
- **Visão Consolidada**: Todos os quartos ocupados em uma tela
- **Detalhes do Hóspede**: Informações completas de contato
- **Período de Estadia**: Datas e dias restantes
- **Status de Pedidos**: Pedidos ativos e histórico
- **Valor Total**: Hospedagem + pedidos
- **Modal Detalhado**: Estatísticas e histórico completo

### 💰 **Gestão Financeira**
- **Contas a Pagar**: Controle de despesas e fornecedores
- **Contas a Receber**: Controle de receitas e clientes
- **Alertas de Vencimento**: Notificações visuais
- **Resumos Financeiros**: Totais e estatísticas
- **Controle de Status**: Pendente, pago, recebido, vencido

## Melhorias Futuras Sugeridas

1. **Relatórios Avançados**: Relatórios detalhados em PDF
2. **Dashboard Financeiro**: Gráficos e análises
3. **Notificações**: Alertas por email ou SMS
4. **Integração**: APIs para sistemas de pagamento
5. **Mobile App**: Aplicativo móvel nativo
6. **Backup**: Sistema automático de backup
7. **Multi-usuário**: Sistema de permissões
8. **API Externa**: Integração com sistemas contábeis

