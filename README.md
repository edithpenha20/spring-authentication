# mudi-parte1
Mudi - Spring MVC

# Spring MVC: e-commerce com Thymeleaf e Bootstrap

Web App de um e-commerce para oferta de produtos usados, utilizando as seguintes tecnologias:
- Java 11;
- Spring MVC;
- Spring Boot;
- Spring Data;
- Spring Security;
- Thymeleaf;
- Bootstrap.


# Como funcionou o processo de requisição do usuário nessa aplicação:

Conforme mostra o diagrama abaixo, o usuário faz uma requisição para "/home"(http://localhost:8080/home), que é mapeada para a classe "HomeController"; nessa classe o método @GetMapping recebe a requisição e a processa por meio da classe "PedidoRepository", esta faz a busca dos pedidos no banco de dados através do método findAll(); usando o JPA este método mapeia os dados registrados na tabela e os lista em uma lista de pedidos (List< Pedido > pedidos); essa lista de pedidos é adicionado no model (HomeController) que envia essa lista de pedidos para home.html, nesse momento o Thymeleaf que está gerando o HTML envia a resposta para o usuário.

### Processo de requisição do usuário
![diagrama de requisicao do usuario](https://github.com/edithpenha20/mudi-parte1/blob/main/Diagrama%20em%20branco.png)

**URL da aplicação**
http://localhost:8080/home
