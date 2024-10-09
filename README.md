# Projeto Spring WebFlux com R2DBC

Este projeto é uma API reativa utilizando **Spring WebFlux** e **R2DBC** (Reactive Relational Database Connectivity) para comunicação com o banco de dados. Ele é construído com uma arquitetura não-bloqueante, focada em alta escalabilidade e performance.

## Tecnologias Utilizadas
- **Java 17** ou superior ou teste
- **Spring Boot** 2.5+
- **Spring WebFlux**
- **R2DBC** (PostgreSQL ou outro banco suportado)
- **Reactor** para manipulação de fluxos reativos
- **Docker** e **Docker Compose** para ambientes de contêineres
- **Maven** como gerenciador de dependências

## Requisitos

Antes de rodar o projeto, certifique-se de ter instalado:
- **Java 17** ou superior
- **Docker** e **Docker Compose**
- **Maven** (opcional, se desejar rodar o projeto localmente sem Docker)

## Configuração do Banco de Dados

Estamos utilizando **R2DBC** para conectar com um banco de dados relacional de forma reativa. O arquivo `application.yml` contém as configurações para o banco de dados.

```yaml
spring:
  r2dbc:
    url: r2dbc:postgresql://localhost:5432/meubanco
    username: usuario
    password: senha
