# CursoMVC
Curso MVC - Bootcamp

# Entity Framework
O Entity Framework é um ORM(Mapeador relacional de objeto) que permite que os desenvolvedores de .NET trabalhem com um banco de dados usando objetos .NET. Elimina a necessidade da marioria do código de acesso a dados que os desenvolvedores geralmente precisam gravar.
O Entity Framework possui três linhas pricipais de utilização:
  - Database First
  - Model First
  - Code First

# Databese First
A  abordagem DataBase First parte de um banco de dados existente e assim você deve ter um banco de dados e as tabelas já criadas e prontas para uso.

# Model First
O Model First nos permite gerar primeiro um modelo e a partir dele gerar nossa base de dados.
Essa montagem de modelo é feita através do EDM Designer, utilizando os componentes que ele nos disponibiliza, sendo as mais comuns "Entity" e "Association".

# Code First
Na abordagem Code First você cria primeiro as suas classes de entidade e deixa para o Entity Framework a responsabilidade de criar o banco de dados.
Essas classes são conhecidas como classes POCO(Plan Old CLR Objects) que são classes que utilizam apenas os tipos do .NET Framework sendo independente de qualquer outro framework inclusive do "Entity", essas classes podem ser utilizadas por outros projetos que utilizem ou não o Entity Framework.

# Data Annotations
O Data Annotations é um recurso que permite que você adicione atributos e métodos em nossas classes para alterar convenções padrão e personalizar alguns comportamentos.
## Principais Atributos
  - **Required:** Significa campo obrigatório.
  - **RegularExpression:** Valida o campo por expressão regular.
  - **Display:** Nome a ser mostrado em todas as interfaces de usuário.
  - **StringLength:** Determina a quantidade máxima de caracteres que poderá ser informada.
  - **MinLength:** Determina a quantidade mínima de caracteres que poderá ser informado.
  - **DisplayFormat:** Formato a ser exibido nas interfaces de usuário.
  - **Range:** Define a faixa de dados aceita pela propriedade.

# Migrations
O Migrations é um recurso que oferece uma maneira de atualizar de forma incremental o esquema de banco de dados para manter em sincronia com o modelo de classe do seu projeto, preservando os dados existentes no banco de dados.
Com o Migrations também é possível realizar o downgrade caso você deseje voltar o seu banco de dados para a versão anterior em que se encontrava, além de manter um historico de alterações.
Antes do Entity Framework contar com suporte ao Migrations, existia apenas três estratégias para a criação de banco de dados, quais sejam:
  - CreateDatabaseIfNotExists
  - DropCreateDatabaseAlways
  - DropCreateDatabaseIfModelChanges
## CreateDatabaseIfNotExists
Nessa estratégia o Entity Framework somente cria o banco de dados se ele não existir, ou seja, se você estiver utilizando essa estratégia e realizar uma alteração no seu modelo de classes, você teria que remover o seu banco de dados e cria-lo novamente, perdendo, assim, todos os seus dados.
## DropCreateDatabaseAlways
Nesse modelo o Entity Framework apaga o banco de dados e o recria sempre que o projeto é executado, fazendo com que você perca todos os seus dados ao inicia-lo.
## DropCreateDatabaseIfModelChanges
Nessa estratégia o Entity Framework apaga o seu banco de dados e o cria sempre que identificar uma alteração no seu modelo de classes, isso também faz com que você perca todos os seus dados, porém apenas quando você realizar a alteração do seu modelo.

# O que é API?

A sigla API em português significa "interface de programação de aplicações".
As APIs são uma forma de realizar a integração entre sistemas, mesmo que esses possuam linguagens de programação diferentes.
Um exemplo de API é o Google Maps que é utilizado por empresas de Hotel em que é disponibilizada dentro do site da a empresa a localização em que ele fica.

# O que é REST?

O REST é um conjunto de princípios que quando aplicados de maneira correta em uma aplicação, a beneficia com a arquitetura e padrões da pŕopria web.
Uma aplicação que é capaz de aplicar tais principios é chamada de RESTful.

# Swagger

Quando é preciso consumir uma API existente é necessário conhecer as funcionalidades disponíveis e detalhes de como consumir tal funcionalidade.
Diante dessa necessidade, existe o Swagger que é um projeto composto por algumas ferramentas para auxiliar o desenvolvimento de API em algumas tarefas, como por exemplo a documentação da API.
