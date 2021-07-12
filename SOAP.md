# Serviços Web

Serviços web ou Web Services são soluções para aplicações se comunicarem independente de linguagem, softwares e hardwares utilizados.
Inicialmente Serviços Web foram criados para troca de mensagens, utilizandos a linguagem XML (Extensible Markup Language) sobre o protocolo HTTP sendo indentificado por URI (Uniform Resource Identifier).
Podemos dizer que Serviços Web são API's que se comunicam por meio de redes sobre o procolo HTTP.

## Vantagens:

- Linguagem Comum
- Integração
- Reutilização de implementação
- Segurança
- Custos

## Principais Tecnologias

- SOAP
- REST
- XML
- JSON

## SOAP

- SOAP - Simple Object Access Protocol
- É um protocolo baseado em XML para acessar serviços web, principalmente por HTTP.
- Pode-se dizer que SOAP é uma definição de como serviços web se comunicam.
- Foi desenvolvido para facilitar integrações entre aplicações.

## Vantagens

- Permite integrações entre aplicações, independente de linguagem, pois usa como linguagem comum o XML
- É independente de plataforma e software
- Meio de transporte genérico, ou seja, pode ser usado por outros protocolos além do HTTP.

## XML

- XML - Extensible Markup Language
- É uma linguagem de marcação criada na decada de 90 pela W3C
- Facilita a separação de conteúdo.
- Facilita a separação de conteúdo
- Não tem limitação de criação de tags.
- Linguagem comum para integrações entre aplicações.

## Estrutura SOAP

O SOAP Message possui uma estrututra unica que deve sempre ser seguida.

**SOAP Envelope - é o primeiro elemento do documento e é usado para encapsular toda a mensagem SOAP.**

**SOAP Header - É  o elemento onde possui informações de atributos e metadados da requisição.**

**SOAP Body - É o elemento que contém os detalhes da mensagem.**

Exemplo de MENSAGEM SOAP

```soap
<soap:Envelope xmlns:soap="http://www.w3.org/2003/05/soap-envelope">
	<soap:Header>
	</soap:Header>
	<soap:Body>
		<m:MetodoEndereco xmlns:m="http://www.example.org/endereco">
			<m:Cidade>São Paulo</m:Cidade>
			<m:CEP>07172-200</m:CEP>
			<m:Logradouro>Rua Augusto Hog</m:Logradouro>
			<m:Numero>14</m:Numero>
		</m:Endereco>
	</soap:Body>
</soap:Envelope>	
```

## WSDL

- W3C - Web Services Description Language
- Usado para descrever Web Services, funciona como um contrato do serviços
- A decrição é feito em cum documento XML, onde é descrito o serviço, especificações de acesso, operações e métodos.

## XSD

- XSD - XML Schema Definition
- É um schema no formato XML, usado para definir a estrutura de dados que será validada no XML.
- O XSD funciona como uma documentação de como deve ser montado o SOAP Message (XML) que será enviado através de Web Service.

## REST

- REST - Representational State Transfer
- É um estilo de arquitetura de software que define a implementação de um serviço web
- Podem trabalhar com os formatos XML,JSON ou outros.

## Vantagens

- Permite integrações entre aplicações e também entre cliente e servidor em páginas web e aplicações
-  Utiliza dos métodos HTTP para definir a operação que está sendo efetuada.
- Arquitetura de fácil compreensão.

## API

- API - Application Programming Interface
- São conjuntos de rotinas documentados e disponibilizados por uma aplicação para que outras aplicações possam consumir suas funcionalidades
- Ficou popular com o aumento dos serviços web
- As maiores plataformas de tecnologia, disponibilizam APIs para acessos de suas funcionalidades, algumas delas são: Facebook, Twitter, Telegram, Whatsapp, GitHub...

## Principais Métodos HTTP:

- GET - Solicita a representação de um recurso.
- Post - Solicita a criação de um recurso.
- DELETE - Solicita a exclusão de um recurso.
- PUT - Solicita a atualização de um recurso.

## JSON
- JSON - JavaScript Object Notation
- Fomatação leve utilizada para troca de mensagens entre sistemas.
- Usa-se de uma estrutura de chave e valor e também de listas ordenadas
- Um dos formatos mais populares e mais utilizados para a troa de mensagens entre sistemas.

## CÓDIGO DE ESTADO

- Usado pelo servidor para avisar o cliente sobre o estado da operação solicitada
- **1xx** - Informativo
- **2xx** - Sucesso
- **3xx** - Redirecionamento
- **4xx** - Erro do cliente
- **5xx** - Erro do Servidor
