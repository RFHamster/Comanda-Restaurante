# Comanda de um Restaurante

Este repositório representa meu trabalho final de PDM (Programação para Dispositivos Móveis), que consistia em fazer um catálogo de vendas para um restaurante, utilizando o SQL Lite do Java Android como banco.

Este trabalho foi feito com o auxilio de outros 2 alunos, Gabriel Gama e Waldemar Silva. Os dois ficaram com a parte do front-end do projeto, fazendo o desgin e o alinhamento dos componentes na tela. Minha parte foi o backend do projeto, toda a parte das classes ficaram por minha conta. Assim, a primeira etapa (da minha parte) foi preparar o banco de dados, criando as classes FeedReaderContract (que representa os contratos/tabelas) e FeedDbHelper (que seria o banco de dados) para a manipulação do SQLite, conforme a documentação presente no AndroidStudio. Com o banco pronto, fiz uma espécie de Facade com a classe ComandosBancos, para interagir com as classes de Itens (do catalogo) e Pedido, assim, qualquer um conseguir manipular o banco de dados de uma maneira mais fácil, somente chamando as respectivas funções que já seriam criadas por mim.

//Imagem ComandosBancos

Com o sistema pronto, faltava integrar o mesmo nas telas, assim, criamos as classes TelaCatalogo e TelaPedidos, onde manipulariamos o banco para criar e modificar pedidos e itens. Em uma primeira versão estavamos puxando do banco e inserindo direto em um Map, que posteriormente seria utilizado na ListView para mostrar os itens. Entretanto, após uma conversa com o professor ele nos mostrou a maneira certa de fazer, criando uma classe que funcionaria como um adaptador. Assim, como eu era reponsavel pelo backend, fiz essa mudança e adaptei as classes para funcionar de maneira correta

//Imagens do App
