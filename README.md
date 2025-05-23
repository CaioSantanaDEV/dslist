
# Projeto DSList
Projeto de estudo, disponibilizado pela DevSuperior, desenvolvido para praticar conceitos de backend com Java e Spring Boot, implementando um catálogo de jogos com listas personalizáveis.

## Modelo de domínio DSList
![Modelo de domínio DSList](https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/dslist-model.png)




## Aprendizados Adquiridos
Spring Boot: Criação de projetos, autoconfiguração e starters

JPA/Hibernate: Mapeamento ORM, relacionamentos (@ManyToMany com atributo extra)

Arquitetura em Camadas: Controller → Service → Repository

DTOs: Padrão para transferência de dados e proteção da API

Consultas SQL: Native queries e JPQL personalizadas

Tratamento de Exceções: @ControllerAdvice básico

## Desafios Superados
Relacionamento Many-to-Many com Atributo Extra:

Implementei a tabela Belonging como entidade intermediária para armazenar a posição dos jogos nas listas

Operação de Reordenamento:

Criei um algoritmo para trocar posições de jogos mantendo a consistência

DTOs com ModelMapper:

Aprendi a evitar a exposição direta das entidades

Consultas Personalizadas:

Implementei tanto JPQL quanto native query para casos específicos

## Como Executar Localmente

Requisitos:

Java 17+

Maven 3.8+

Comandos:
```
git clone https://github.com/CaioSantanaDEV/dslist.git
cd dslist
mvn spring-boot:run
```

Endpoints Principais:
```
GET /games          - Lista todos os jogos
GET /lists/{id}     - Busca jogos por lista
PUT /lists/{id}/replacement - Reordena jogos
```
Este projeto representa minha jornada inicial no desenvolvimento backend com Java. Cada linha de código reflete horas de estudo, tentativas e erros, e muita pesquisa!



