# Example application #

A simple Spring Boot application that sports a REST API and does persistence using JPA.

This project is based on Spring Boot's [HATEOAS example](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-hateoas).

# Como executar a aplicação no Desktop # 

# Pré requisitos # 

1. PostgreSQL 10.6
2. Apache Maven 3.5.2
3. git version 2.17.1
4. java version 1.8.0_191

# Como configurar o banco de dados # 

1. Instalar o PostgreSQL DB na maquina local.
$ sudo apt-get install postgresql postgresql-contrib libpq-dev pgadmin3

2. Verificar se o banco de dados foi criado e está rodando.
$ sudo su - postgres
$ psql
$ \l

Output:
List of databases

$ \q
           
3. Conectar com o banco de dados.

$ sudo su - postgres
$ psql

4. Criar o banco de dados

$ create database customerdb;

$ create user springuser with encrypted password 'springuser';

$ grant all privileges on database customerdb to springuser;

$ \q;


# Como configurar a aplicação #

1. Criar o repositório git.

$ mkdir bravit

$ cd bravit

$ git remote add origin https://github.com/bravi-software/teste-arquiteto-bravi.git

2. Clonar o repositório de origem.

$ git clone https://github.com/bravi-software/teste-arquiteto-bravi.git

3. verificar se o diretorio "teste-arquiteto-bravi".

# Como executar os testes da aplicação #

1. No diretorio raiz "bravit" executar.

$ cd teste-arquiteto-bravi

$ mvn clean

$ mvn test

Output: 

[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 18.774 s
[INFO] Finished at: 2019-01-06T10:49:02-02:00
[INFO] Final Memory: 21M/200M
[INFO] ------------------------------------------------------------------------

