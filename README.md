

<br/>Java e refatoração: melhorando códigos com boas práticas<br/>
=================

A aplicação será integrada com uma API externa, que será a responsável por salvar pets e abrigos da aplicação console,
assim como retorná-los quando fizermos a requisição através da aplicação console. Essa API está incluída no formato 
.jar no nosso projeto que vamos utilizar para o curso. E para testar a aplicação console precisamos iniciar o arquivo .jar. 

Para isso, podemos usar o seguinte comando:

java -jar api.jar

## 01. Refatoração

### Nesta aula:
* Aprendemos a extrair código em métodos, com o intuito de melhorar a legibilidade do nosso código, facilitando assim sua manutenção;
* Entendemos o problema do código duplicado e como resolvê-lo para evitar inconsistências no código, caso haja alteração em um ponto do código duplicado e no outro não;
* Vimos que o ideal para resolver o código duplicado é aplicar a reutilização de código, em que o código fica presente em apenas um local e referenciá-lo ao utilizá-lo. Dessa forma, toda manutenção será feita em apenas um local.

## 02. SOLID

* Aprendemos que o S do acrônimo SOLID significa Single Responsability Principle, em português, princípio da responsabilidade única, ou seja, uma classe deve ter um, e somente um, motivo para mudar;
* Separamos nosso código em classes para que ficassem coesas e com apenas uma responsabilidade;
* Criamos classes de configurações para reaproveitá-las nas classes de serviço, evitando assim código duplicado.