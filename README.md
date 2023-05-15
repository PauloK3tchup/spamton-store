# Projeto Integrador - Spamton Store

Alunos: [Paulo César N. Padilha](https://github.com/PauloK3tchup) e [Gabriel Fernandes Domingos](https://github.com/Brobss).

Links do projeto:

- [Documentação (esse documento)](https://github.com/PauloK3tchup/spamton-store-docs)
- [Backend]()
- [Frontend]()

# Situação Problema
Spamton Store é uma loja de produtos variados que está no mercado desde 1997.
Seu fundador e único funcionário é o humilde vendedor Spamton G. Spamton. Os produtos são caseiros (estavam na casa dele) e variam desde frutas e legumes a automóveis e dispositivos perigosos.


Ao chegar na loja, o cliente é recebido por Spamton, que atua como caixa e responsável pelo atendimento ao cliente. Ele se dirige ao balcão e pode visualizar os produtos disponíveis na loja, a fim de escolher o que deseja comprar.

Após selecionar o produto, o cliente faz o pedido com Spamton, que registra a compra. Em seguida, ele se dirige à dispensa ao lado do caixa, para verificar a disponibilidade do item solicitado e retirá-lo do estoque.

Ao retornar ao caixa, Spamton conclui a venda manualmente, entregando o produto diretamente ao cliente. Ele também registra a venda em seu diário, para manter um controle das vendas realizadas.

Dessa forma, o cliente pode finalizar sua compra de maneira rápida e eficiente, com o auxílio de Spamton como caixa e atendente da loja.

<img src="docs/cliente%20no%20balcão.png" width="500" height="500">

Existem diversos fatores atrasando a execução dos serviços de Spamton. Todo o trabalho é feito manualmente, Spamton sempre tem de ir a sua dispensa verificar a disponibilidade do estoque. As vendas e relatórios também são feitas à mão. Estes fatores fazem com que, em dias muito movimentados, Spamton tenha de repetir estes processos manuais diversas vezes, atrasando muito o fluxo de vendas e pessoas na loja, fazendo com que diversos clientes fiquem insatisfeitos com a longa espera. Um software removeria todos esses problemas, ajudando a organizar o estoque e otimizar as vendas.
# Descrição da proposta

O software tem a função de compra e venda de produtos (loja online) pelo lado do cliente e organização do estoque e relatórios pela parte administrativa. O sistema terá dois tipos de usuário: gestor e cliente.

- Gestor: Terá uma conta administrativa. Ele terá acesso ao gerenciamento do estoque, podendo verificar a disponibilidade em tempo real e organizar os itens disponíveis na loja online. O gestor terá acesso aos relatórios das vendas, que serão feitos de forma automática. Também terá acesso aos pedidos dos clientes para organizar as formas de entrega selecionadas pelos mesmos.

- Cliente: O cliente terá acesso à loja online, procurando os produtos disponíveis e podendo comprá-los com diferentes meios de pagamento. A loja online permite que o cliente selecione o tipo de entrega: retirada no local ou entrega em seu endereço. Para ter acesso às funções de compra o cliente terá de criar uma conta no site, informando seu endereço e dados de pagamento.

# Regras de Negócio

- **RN01 - Cadastro de clientes:** O software deve permitir que os clientes criem uma conta na loja online. Os clientes também devem poder fazer login na loja online com suas contas criadas.

- **RN02 - Catálogo de produtos:** O software deve manter um catálogo de produtos disponíveis para venda na loja online, permitindo que os clientes visualizem os produtos e selecionem os que desejam comprar.

- **RN03 - Compra Restrita a Usuários Autenticados:** O software deve permitir que apenas usuários autenticados façam compras na loja online.

- **RN04 - Carrinho de compras:** O software deve permitir que os clientes adicionem produtos ao carrinho de compras, selecionando a quantidade de cada produto e a forma de entrega. O software deve calcular automaticamente o valor total da compra.

- **RN05 - Compra de produtos:** O software deve permitir que os clientes façam compras na loja online, selecionando a forma de pagamento e a forma de entrega.

- **RN06 - Controle de estoque:** O software deve manter um registro atualizado do estoque de produtos disponíveis para venda e alertar o gestor quando a quantidade mínima de um produto for atingida.

- **RN07 - Relatórios de vendas:** O software deve gerar automaticamente relatórios de vendas diárias, semanais e mensais para o gestor, permitindo o acompanhamento do desempenho da loja e identificação de tendências e oportunidades de melhoria.

- **RN08 - Processamento de pagamento:** O software deve permitir que os clientes façam pagamentos online de forma segura e eficiente, aceitando diferentes formas de pagamento, como cartão de crédito, transferência bancária, PIX e boleto bancário.

- **RN08 - Gestão de pedidos:** O software deve permitir que o gestor gerencie os pedidos dos clientes, organizando as formas de entrega selecionadas e mantendo os clientes informados sobre o status de seus pedidos.

- **RN10 - Atualizações de produtos:** O gestor deve ser capaz de atualizar o catálogo de produtos disponíveis na loja online, incluindo novos produtos e removendo itens que não estão mais disponíveis.

- **RN11 - Política de devolução:** A loja deve ter uma política clara de devolução de produtos, informando aos clientes os prazos e condições para devolução e reembolso de produtos.

- **RN12 - Histórico de compras:** O software deve manter um histórico das compras realizadas pelos clientes, permitindo que eles visualizem suas compras anteriores e facilitando futuras compras.

- **RN13 - Descontos e promoções:** O software deve permitir a criação de descontos e promoções em produtos selecionados, bem como a emissão de cupons de desconto para os clientes.

- **RN14 - Avaliação dos Clientes** - O software deve permitir que os clientes avaliem os produtos que compraram, permitindo que outros clientes visualizem as avaliações e comentários.

# Requisitos Funcionais

## Entradas

- **R.F. 01 - Cadastro de clientes:** O software deve permitir que os clientes criem uma conta na loja online.<ins>Dados necessários:</ins> Nome, CPF, endereço, telefone, e-mail, senha. <ins>Usuários:</ins> todos.

- **R.F. 02 - Gestão de Estoque:** O software deve permitir que o gestor gerencie o estoque de produtos disponíveis na loja online, permitindo a adição de novos produtos e a remoção de produtos que não estão mais disponíveis. <ins>Dados necessários:</ins> Nome, descrição, preço, quantidade, categoria. <ins>Usuários:</ins> gestor.

- **R.F. 03 - Cadastro de métodos de pagamento:** O software deve permitir que o usuário cadastre novos meios de pagamento em sua conta. <ins>Dados necessários:</ins> Nome do cartão, número do cartão, data de validade, código de segurança. <ins>Usuários:</ins> todos.

- **R.F. 04 - Avaliações:** O software deve permitir que os clientes avaliem os produtos que compraram, permitindo que outros clientes visualizem as avaliações e comentários. <ins>Dados necessários:</ins> Avaliação, comentário. <ins>Usuários:</ins> todos.

## Processos

- **R.F. 05 - Gestão de Pedidos:** O software deve permitir que o gestor gerencie os pedidos dos clientes, organizando as formas de entrega selecionadas e mantendo os clientes informados sobre o status de seus pedidos. <ins>Dados necessários:</ins> código do pedido, código da conta do usuário. <ins>Usuários:</ins> gestor.

- **R.F. 06 - Pesquisa:** O software deve permitir que os clientes pesquisem produtos na loja online, filtrando os resultados por categoria, preço e disponibilidade. <ins>Dados necessários:</ins> Nome do produto, categoria, preço, disponibilidade. <ins>Usuários:</ins> todos.

- **R.F. 07 - Carrinho:** O software deve permitir que os clientes adicionem produtos ao carrinho de compras, selecionando a quantidade de cada produto e a forma de entrega. O software deve calcular automaticamente o valor total da compra. <ins>Dados necessários:</ins> código do produto, quantidade, forma de entrega. <ins>Usuários:</ins> todos.

- **R.F. 08 - Compra de produtos** - O software deve permitir que os clientes façam compras na loja online, selecionando a forma de pagamento e a forma de entrega. <ins>Dados necessários:</ins> dados do método de pagamento selecionado, código da conta do usuário. <ins>Usuários:</ins> todos.

- **R.F. 09 - Débito em conta:** O software deve permitir que os clientes façam pagamentos online de forma segura e eficiente, aceitando diferentes formas de pagamento, como cartão de débito, transferência bancária, PIX e boleto bancário. <ins>Dados necessários:</ins> código do pedido, código da conta do usuário. <ins>Usuários:</ins> todos.

- **R.F. 10 - Crédito em conta:** O software deve permitir que os clientes façam pagamentos online de forma segura e eficiente, aceitando cartão de crédito. <ins>Dados necessários:</ins> código do pedido, código da conta do usuário. <ins>Usuários:</ins> todos.

- **R.F. 11 - Histórico de Compras:** O software deve manter um histórico das compras realizadas pelos clientes, permitindo que eles visualizem suas compras anteriores e facilitando futuras compras. <ins>Dados necessários:</ins> código do pedido, código da conta do usuário. <ins>Usuários:</ins> todos.

- **R.F. 12 - Autenticação:** O software deve permitir que os usuários façam login na loja online com suas contas criadas. <ins>Dados necessários:</ins> e-mail, senha. <ins>Usuários:</ins> todos.

## Saídas

- **R.F. 13 - Exibição de Produtos:** O software deve exibir os produtos disponíveis na loja online, permitindo que os clientes visualizem os detalhes de cada produto. <ins>Dados necessários:</ins> Nome, descrição, preço, quantidade, categoria. <ins>Usuários:</ins> todos.

- **R.F. 14 - Relatórios:** O software deve gerar automaticamente relatórios de vendas diárias, semanais e mensais para o gestor, permitindo o acompanhamento do desempenho da loja e identificação de tendências e oportunidades de melhoria. <ins>Dados necessários:</ins> código do pedido, código da conta do usuário. <ins>Usuários:</ins> gestor.

# Requisítos Não Funcionais

## Requisitos de Qualidade

- **R.N.F. 01 - Navegador homologado:** O sistema deverá ser homologado para Google Chrome, Microsoft Edge, Opera e Firefox.

- **R.N.F. 02 - Disponibilidade:** O sistema deverá estar disponível 24 horas por dia, 7 dias por semana.

- **R.N.F. 03 - Segurança:** O sistema deverá ser seguro, evitando que dados sensíveis dos clientes sejam expostos a terceiros.

- **R.N.F. 04 - Responsividade:** O sistema deverá ser responsivo, permitindo que os clientes acessem a loja online de qualquer dispositivo, como computadores, tablets e smartphones.

- **R.N.F. 05 - Desempenho:** O software deve ser capaz de processar um grande número de transações simultaneamente sem diminuir significativamente o desempenho. Por exemplo, o sistema deve ser capaz de lidar com picos de tráfego durante as promoções de vendas da loja sem sofrer interrupções ou quedas de performance.

- **R.N.F. 06 - Usabilidade:** O software deve ser fácil de usar para os clientes, com interface intuitiva e instruções claras. Além disso, o sistema deve ser responsivo e compatível com dispositivos móveis, permitindo que os clientes façam compras de qualquer lugar, a qualquer hora.

- **R.N.F. 07 - Manutenção:** O software deve ser facilmente mantido e atualizado, permitindo que os desenvolvedores adicionem novos recursos e corrijam bugs sem interromper o funcionamento da loja online.

- **R.N.F. 08 - Arquitetura:** A arquitetura que será utilizada para criação do sistema será Rest.

## Restrições

- **R.N.F. 09 - Segurança de Vendas:** O sistema deve garantir que apenas usuários autenticados e com todos os dados obrigatórios cadastrados possam realizar compras na loja online.

- **R.N.F. 10 - Restrição de Acesso:** O sistema deve garantir que apenas o gestor tenha acesso às funcionalidades de gestão de estoque, pedidos e relatórios.
