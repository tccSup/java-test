# Desafio Back End Java na DoroTech

Somos uma empresa com clientes que atuam em vários segmentos do mercado, com diferentes tecnologias, culturas e desafios.

Gostamos de compor nossos times com profissionais multidisciplinares, que tenham alta capacidade de aprendizado, sejam detalhistas, resilientes, questionadores e curiosos. Você, como Java Developer, será o responsável por implementar, dar manutenção, aplicar correções e propor soluções em projetos de software.

## Requisitos do desafio:
```
1. Criar um código que execute um CRUD(Create, Read, Update, Delete) em uma tabela para gerenciar produtos eletrônicos.
2. Use um banco NoSQL(DynamoDB é um diferencial).
3. Utilizar Spring como framework(Quarkus é um diferencial).
4. Dados da tabela a ser criada no banco:
    - Products:
        name,
        description,
        price,
        amount.


Seja criativo! fazer o melhor não é ser complexo.
``` 

## Dicas e Informações Valiosas
```
O que gostaríamos de ver em seu teste:
    
    Convenção de nome em classes, objetos, variáveis, métodos e etc.
    Faça commits regulares. Eles são melhores do que um commit gigantesco. Gostaríamos de ver commits organizados e padronizados, então capriche neles!
    Bônus 1 Quarkus & AWS, implementação de uma lambda AWS utilizando framework Quarkus
    Bônus 2 Testes automatizados
    Observação: Nenhum dos itens acima é obrigatório.

O que o seu Teste não deve ter:
    Saber que não foi você quem implementou o projeto.
    Várias bibliotecas instaladas sem uso.
    Falta de organização de código.
    Falta de documentação.
    Nome de variáveis sem sentido ou sem padrão de nomes.
    Histórico de commits desorganizado e despadronizado.

Boa Sorte!!
```

## Itens obrigatórios
```
1. Possibilitar a criação de um novo produto
2. Possibilitar consulta de todos os produtos no banco de dados.
3. Possibilitar consultar um produto específico pelo id.
4. Permitir a exclusão de um produto.
5. Persistir os dados na base.
```

## Itens desejáveis
```
1. Criação de Testes unitários.
2. Utilização de alguma ferramenta AWS(API Gateway, Lambda, SQS, SNS, EC2,..).
3. Docker.
4. Utilização de algum padrão de projeto.
```

### Instruções para entrega
```
1. Fazer um fork desse repositório

2. Criar um branch com o seu primeiro e último nome
git checkout -b joao-silva

3. Escreva a documentação da sua aplicação
Você deve, substituir o conteúdo do arquivo README.md e escrever a documentação da sua aplicação, com os seguintes tópicos:
    - Projeto: Descreva o projeto e como você o executou. Seja objetivo.
    - Tecnologias: Descreva quais tecnologias foram utilizadas, enumerando versões (se necessário) e os links para suas documentações, quais bibliotecas instalou e porque.
Como compilar e rodar: Descreva como compilar e rodar sua aplicação.

4. Faça uma Pull Request
Após implementada a solução, crie uma pull request com o seu projeto para esse repositório, avise o recrutador.
```


# dorotech-desafio

This project uses Quarkus, the Supersonic Subatomic Java Framework.

If you want to learn more about Quarkus, please visit its website: https://quarkus.io/ .

## Running the application in dev mode

You can run your application in dev mode that enables live coding using:

```shell script
./gradlew quarkusDev
```

> **_NOTE:_**  Quarkus now ships with a Dev UI, which is available in dev mode only at http://localhost:8080/q/dev/.

## Packaging and running the application

The application can be packaged using:

```shell script
./gradlew build
```

It produces the `quarkus-run.jar` file in the `build/quarkus-app/` directory.
Be aware that it’s not an _über-jar_ as the dependencies are copied into the `build/quarkus-app/lib/` directory.

The application is now runnable using `java -jar build/quarkus-app/quarkus-run.jar`.

If you want to build an _über-jar_, execute the following command:

```shell script
./gradlew build -Dquarkus.package.type=uber-jar
```

The application, packaged as an _über-jar_, is now runnable using `java -jar build/*-runner.jar`.

## Creating a native executable

You can create a native executable using:

```shell script
./gradlew build -Dquarkus.package.type=native
```

Or, if you don't have GraalVM installed, you can run the native executable build in a container using:

```shell script
./gradlew build -Dquarkus.package.type=native -Dquarkus.native.container-build=true
```

You can then execute your native executable with: `./build/dorotech-desafio-1.0-SNAPSHOT-runner`

If you want to learn more about building native executables, please consult https://quarkus.io/guides/gradle-tooling.

## Related Guides

- SmallRye OpenTracing ([guide](https://quarkus.io/guides/opentracing)): Trace your services with SmallRye OpenTracing
- Hibernate Validator ([guide](https://quarkus.io/guides/validation)): Validate object properties (field, getter) and
  method parameters for your beans (REST, CDI, Jakarta Persistence)
- RESTEasy Reactive ([guide](https://quarkus.io/guides/resteasy-reactive)): A Jakarta REST implementation utilizing
  build time processing and Vert.x. This extension is not compatible with the quarkus-resteasy extension, or any of the
  extensions that depend on it.
- SmallRye OpenAPI ([guide](https://quarkus.io/guides/openapi-swaggerui)): Document your REST APIs with OpenAPI - comes
  with Swagger UI
- Jacoco - Code Coverage ([guide](https://quarkus.io/guides/tests-with-coverage)): Jacoco test coverage support
- Hibernate ORM with Panache ([guide](https://quarkus.io/guides/hibernate-orm-panache)): Simplify your persistence code
  for Hibernate ORM via the active record or the repository pattern
- Agroal - Database connection pool ([guide](https://quarkus.io/guides/datasource)): Pool JDBC database connections (
  included in Hibernate ORM)
- SmallRye Metrics ([guide](https://quarkus.io/guides/smallrye-metrics)): Expose metrics for your services
- JDBC Driver - PostgreSQL ([guide](https://quarkus.io/guides/datasource)): Connect to the PostgreSQL database via JDBC

## Provided Code

### Hibernate ORM

Create your first JPA entity

[Related guide section...](https://quarkus.io/guides/hibernate-orm)

[Related Hibernate with Panache section...](https://quarkus.io/guides/hibernate-orm-panache)

### RESTEasy Reactive

Easily start your Reactive RESTful Web Services

[Related guide section...](https://quarkus.io/guides/getting-started-reactive#reactive-jax-rs-resources)
