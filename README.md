#  TradeCore API - Sistema de Gestão de Estoque e Vendas

![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)

Uma API RESTful corporativa desenvolvida em **C# (.NET 8)** e **MySQL** para resolver o problema de dessincronização entre vendas e controle de estoque em pequenas e médias empresas.

##  Funcionalidades

- **Autenticação Segura:** Geração de tokens JWT com níveis de acesso (Admin/Vendedor).
- **Controle de Estoque:** CRUD de produtos com validação de estoque mínimo.
- **Processamento de Vendas:** Registro de pedidos com baixa automática no estoque de forma transacional.
- **Relatórios Gerenciais:** Geração de dados consolidados de vendas por período.
- **Documentação Interativa:** Interface Swagger disponível para testes das rotas.

##  Arquitetura e Boas Práticas
Este projeto foi construído focando em escalabilidade e manutenção:
- **Repository Pattern:** Separação da lógica de acesso a dados.
- **DTOs (Data Transfer Objects):** Prevenção de over-posting e isolamento das entidades de domínio.
- **Global Exception Handling:** Middleware customizado para padronização de respostas de erro.
- **Entity Framework Core (Code-First):** Migrations automatizadas.

##  Como rodar localmente

1. Clone o repositório:
   ```bash
   git clone [https://github.com/Lucasfrrb/TradeCore-API.git](https://github.com/Lucasfrrb/TradeCore-API.git)
