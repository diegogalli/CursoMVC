# CursoMVC
Curso MVC

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
