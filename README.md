# Projeto Integrador - Spamton Store

Alunos: [Paulo César N. Padilha](github.com/PauloK3tchup) e [Gabriel Fernandes Domingos](https://st.depositphotos.com/1518767/4823/i/950/depositphotos_48239019-stock-photo-businessman-shrugging-shoulders.jpg).

Links do projeto:

-   [Documentação (esse documento)](https://github.com/PauloK3tchup/spamton-store-docs)
-   [Backend](lol)
-   [Frontend](bruh)

# Introdução

Spamton Store é uma loja de produtos variados que está no mercado desde 1997. 
Seu fundador e único funcionário é o humilde vendedor Spamton G. Spamton. Os produtos são caseiros (estavam na casa dele) e variam desde frutas e legumes a automóveis e dispositivos perigosos.

# Situação Problema


O cliente se desloca até a casa de Spamton e entra pela porta. Ao entrar na casa o cliente se desloca até o balcão no qual Spamton trabalha como caixa, e nele pode ver ou solicitar um item disponível.

![Cliente no balcão de Spamton](docs/cliente%20no%20balc%C3%A3o.png "Cliente & Spamton")

 Spamton anota o pedido e vai até a dispensa ao lado verificar a disponibilidade do item solicitado e retira-lo do estoque. Spamton retorna ao caixa e conclui a venda manualmente, entregando o produto diretamente ao cliente e anotando a venda em seu diário. 

# Conclusão

Existem diversos fatores atrasando a execução dos serviços de Spamton. Todo o trabalho é feito manualmente, Spamton sempre tem de ir a sua dispensa verificar a disponibilidade do estoque. As vendas e relatórios também são feitas à mão. Estes fatores fazem com que, em dias muito movimentados, Spamton tenha de repetir estes processos manuais diversas vezes, atrasando muito o fluxo de vendas e pessoas na loja, fazendo com que diversos clientes fiquem insatisfeitos com a longa espera. Um software removeria todos esses problemas, ajudando a organizar o estoque e otimizar as vendas.

# Descrição da proposta

O software tem a função de compra e venda de produtos (loja online) pelo lado do cliente e organização do estoque e relatórios pela parte administrativa. O sistema terá dois tipos de usuário: gestor e cliente.

- Gestor: Terá uma conta administrativa. Ele terá acesso ao gerenciamento do estoque, podendo verificar a disponibilidade em tempo real e organizar os itens disponíveis na loja online. O gestor terá acesso aos relatórios das vendas, que serão feitos de forma automática. Também terá acesso aos pedidos dos clientes para organizar as formas de entrega selecionadas pelos mesmos.

- Cliente: O cliente terá acesso à loja online, vendo os produtos disponíveis e podendo compra-los com diferentes meios de pagamento, desde cartão de crédito até pagamento no local. A loja online permite que o cliente selecione o tipo de entrega: retirada no local ou entrega em seu endereço. Para ter acesso as funções de compra o cliente terá de criar uma conta no site, informando seu endereço e dados de pagamento.  
