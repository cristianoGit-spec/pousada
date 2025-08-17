Funcionalidades Principais

1. Dashboard Principal
•Visão geral da ocupação dos quartos
•Alertas de estoque baixo
•Pedidos pendentes
•Consumo do frigobar
•Atividades recentes do sistema

2. Dashboard de Quartos ⭐ NOVA FUNCIONALIDADE
•Visão em Grid: Todos os 40 quartos exibidos em formato de grade
•Status Visual: Quartos ocupados (vermelho) e vagos (verde)
•Estatísticas em Tempo Real:
•Total de quartos: 40
•Quartos ocupados: 3
•Quartos vagos: 37
•Taxa de ocupação: 7.5%
•Quartos com pedidos ativos: 2
•Informações por Quarto:
•Número do quarto
•Tipo (solteiro, casal, duplo)
•Status (ocupado/vago)
•Nome do hóspede (se ocupado)
•Dias restantes da estadia
•Indicador de pedidos ativos
•Modal de Detalhes (para quartos ocupados):
•Informações completas do hóspede
•Dados da estadia (check-in, check-out, duração)
•Resumo financeiro detalhado
•Estatísticas de pedidos

3. Quartos Ocupados
•Visualização detalhada dos quartos atualmente ocupados
•Detalhes completos do hóspede (nome, documento, contato)
•Período de estadia (check-in, check-out, dias restantes)
•Status de pedidos ativos por quarto
•Histórico completo de pedidos do hóspede
•Valor total da estadia (hospedagem + pedidos)

4. Controle de Estoque
•Cadastro de produtos (alimentos, bebidas, produtos de limpeza)
•Controle de entrada e saída de produtos
•Alertas automáticos para estoque baixo
•Relatórios de movimentação
•Categorização por tipo de produto

5. Sistema de Frigobar
•Cadastro de itens do frigobar com preços
•Registro de consumo por quarto
•Controle automático de estoque
•Relatórios de consumo por quarto
•Histórico detalhado de consumo

6. Acompanhamento de Pedidos
•Criação de pedidos por quarto/hóspede
•Controle de status (pendente, em preparo, entregue, cancelado)
•Cálculo automático de valores
•Histórico completo de pedidos
•Observações especiais

7. Sistema de Reservas
•Cadastro de quartos (solteiro, casal, duplo)
•Gestão de hóspedes
•Controle de disponibilidade
•Check-in e check-out
•Cálculo de diárias
•Relatórios de ocupação

8. Contas a Pagar
•Registro de despesas e fornecedores
•Controle de vencimentos e pagamentos
•Alertas para contas vencidas
•Marcação de contas como pagas
•Resumo financeiro (total pendente, pago, vencidas)
•Histórico completo de pagamentos

9. Contas a Receber
•Registro de receitas e clientes
•Controle de recebimentos
•Alertas para contas em atraso
•Marcação de contas como recebidas
•Resumo financeiro (total a receber, recebido, em atraso)
•Integração com hospedagens e serviços

Tecnologias Utilizadas
Backend
•Flask: Framework web Python
•SQLAlchemy: ORM para banco de dados
•SQLite: Banco de dados
•Flask-CORS: Suporte a CORS
Frontend
•React: Biblioteca JavaScript
•React Router: Navegação entre páginas
•Tailwind CSS: Framework CSS
•Shadcn/UI: Componentes de interface
•Lucide React: Ícones
Estrutura do Banco de Dados
Tabelas Principais
•produtos: Controle de estoque geral
•movimentacoes_estoque: Histórico de movimentações
•quartos: Cadastro de quartos
•hospedes: Cadastro de hóspedes
•reservas: Controle de reservas
•itens_frigobar: Produtos do frigobar
•frigobar_consumo: Consumo do frigobar
•pedidos: Pedidos dos clientes
•itens_pedido: Itens dos pedidos
•contas_a_pagar: Controle de despesas
•contas_a_receber: Controle de receitas
Como Usar o Sistema
Acesso
O sistema está disponível em: https://60h5imc0pe18.manus.space
Navegação
O sistema possui 9 seções principais acessíveis pelo menu superior:
1.Dashboard: Visão geral do sistema
2.Dashboard Quartos: Visão em grid de todos os quartos ⭐ NOVO
3.Quartos Ocupados: Detalhes dos quartos ocupados
4.Estoque: Controle de produtos
5.Frigobar: Gestão do frigobar
6.Pedidos: Acompanhamento de pedidos
7.Reservas: Sistema de reservas
8.Contas a Pagar: Gestão de despesas
9.Contas a Receber: Gestão de receitas

Fluxo de Trabalho Recomendado

1.Configuração Inicial
•Cadastre os 40 quartos da pousada
•Cadastre os produtos do estoque
•Configure os itens do frigobar

2.Operação Diária
•Verifique o dashboard principal para alertas
•Use o Dashboard de Quartos para visão geral da ocupação ⭐ NOVO
•Monitore quartos ocupados e seus pedidos
•Processe novos pedidos
•Registre consumo do frigobar
•Gerencie check-ins e check-outs
•Controle contas a pagar e receber

3.Controle Financeiro
•Registre despesas (fornecedores, contas)
•Monitore recebimentos de hospedagens
•Acompanhe vencimentos e atrasos
•Gere relatórios financeiros

4.Controle de Estoque
•Registre entradas de produtos
•Monitore alertas de estoque baixo
•Faça reposições quando necessário

Características Técnicas
•Responsivo: Funciona em desktop e mobile
•Tempo Real: Atualizações instantâneas
•Seguro: Validações no frontend e backend
•Escalável: Arquitetura preparada para crescimento
•Intuitivo: Interface amigável e fácil de usar
•Completo: Gestão integrada de todas as operações
•Visual: Dashboard de quartos com interface moderna

Nova Funcionalidade: Dashboard de Quartos

🏨 Visão em Grid

•Layout Responsivo: Grid adaptável para diferentes tamanhos de tela
•Cores Intuitivas: Verde para quartos vagos, vermelho para ocupados
•Informações Rápidas: Status, tipo, hóspede e pedidos em cada card

📊 Estatísticas em Tempo Real
•Total de Quartos: 40 quartos cadastrados
•Ocupação Atual: 3 quartos ocupados (7.5%)
•Quartos Vagos: 37 quartos disponíveis
•Pedidos Ativos: 2 quartos com pedidos pendentes

🔍 Modal de Detalhes
•Informações do Hóspede: Nome, documento, telefone, email
•Dados da Estadia: Check-in, check-out, dias de estadia, dias restantes
•Resumo Financeiro: Total de pedidos, pedidos pendentes, gasto em pedidos, valor total da estadia

🎨 Design Moderno

•Interface Limpa: Cards bem organizados e fáceis de ler
•Ícones Intuitivos: Representação visual dos tipos de quarto
•Hover Effects: Interações suaves ao passar o mouse
•Modal Responsivo: Detalhes completos em janela modal

Benefícios do Sistema

Para Gestores
•Visão Completa: Dashboard de quartos oferece visão instantânea da ocupação
•Controle Financeiro: Gestão integrada de receitas e despesas
•Eficiência Operacional: Todos os processos em um só lugar
•Relatórios Instantâneos: Informações em tempo real

Para Funcionários
•Interface Intuitiva: Fácil de usar e aprender
•Acesso Rápido: Informações importantes sempre visíveis
•Processo Simplificado: Fluxos de trabalho otimizados
•Menos Erros: Validações automáticas

Para Hóspedes
•Atendimento Ágil: Funcionários com acesso rápido às informações
•Pedidos Organizados: Sistema eficiente de acompanhamento
•Check-in/out Rápido: Processo otimizado

Melhorias Futuras Sugeridas

1.Relatórios Avançados: Relatórios detalhados em PDF
2.Dashboard Financeiro: Gráficos e análises avançadas
3.Notificações Push: Alertas em tempo real
4.Integração: APIs para sistemas de pagamento
5.Mobile App: Aplicativo móvel nativo
6.Backup Automático: Sistema de backup em nuvem
7.Multi-usuário: Sistema de permissões e roles
8.API Externa: Integração com sistemas contábeis
9.Reservas Online: Portal de reservas para clientes
10.Analytics: Relatórios de ocupação e receita
Conclusão

O sistema agora oferece uma solução completa e moderna para gestão de pousadas, 
com destaque para o novo Dashboard de Quartos que proporciona uma visão visual 
e intuitiva de toda a operação. A interface responsiva e as funcionalidades
integradas tornam o sistema uma ferramenta poderosa para otimizar a gestão hoteleira.

