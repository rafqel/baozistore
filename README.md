# 🥟 Baozi Store API

![Java](https://img.shields.io/badge/Java-17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2+-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![H2 Database](https://img.shields.io/badge/H2_Database-003545?style=for-the-badge&logo=database&logoColor=white)
![Maven](https://img.shields.io/badge/Apache_Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge)

> API REST desenvolvida para o controle básico de clientes, produtos e pedidos da **Baozi Store** (loja de pãezinhos chineses).

Este projeto foi desenvolvido como requisito para avaliação da disciplina de **Desenvolvimento Web Back-End** do curso de Análise e Desenvolvimento de Sistemas do Centro Universitário Internacional **UNINTER**.

---

## 📖 Sobre o Projeto

O sistema foi construído utilizando os princípios de APIs REST e a arquitetura MVC do Spring. Ele permite o cadastro e gerenciamento de clientes, produtos e a realização de pedidos simples (onde um cliente compra um produto em determinada quantidade).

### 🏗️ Arquitetura e Estrutura
O projeto segue o padrão de camadas recomendado pelo ecossistema Spring:
*   **`model`**: Contém as entidades JPA (`Cliente`, `Produto`, `Pedido`).
*   **`repository`**: Interfaces que estendem `JpaRepository` para comunicação com o banco de dados.
*   **`controller`**: Classes responsáveis por expor os endpoints REST e receber as requisições HTTP.

---

## 🛠️ Tecnologias Utilizadas

*   **Java 17** (Linguagem base)
*   **Spring Boot 3** (Framework principal)
*   **Spring Web** (Criação dos endpoints REST)
*   **Spring Data JPA** (Persistência de dados)
*   **H2 Database** (Banco de dados relacional em memória)
*   **Lombok** (Redução de código boilerplate)
*   **Maven** (Gerenciador de dependências)

---

## ⚙️ Como Executar o Projeto

### Pré-requisitos
Você vai precisar ter instalado em sua máquina:
*   [Java JDK 17](https://adoptium.net/) ou superior.
*   [Git](https://git-scm.com/) (opcional, para clonar).
*   Uma IDE de sua preferência (IntelliJ IDEA, VS Code, Eclipse).

### Passo a passo
1. Clone o repositório para a sua máquina:
   git clone https://github.com/rafqel/baozistore.git

2. Abra a pasta do projeto na sua IDE e aguarde o download das dependências do Maven.
3. Execute a classe principal `BaozistoreApplication.java`.
4. A API estará rodando localmente no endereço: `http://localhost:8080`.

*(Opcional: O console do banco H2 pode ser acessado em `http://localhost:8080/h2-console`)*

---

## 🔗 Documentação dos Endpoints

Abaixo estão listados os endpoints disponíveis na API.

### 👤 Clientes
| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `POST` | `/clientes` | Cadastra um novo cliente |
| `GET` | `/clientes` | Lista todos os clientes |
| `GET` | `/clientes/{id}` | Busca um cliente específico pelo ID |
| `DELETE` | `/clientes/{id}` | Remove um cliente do sistema |

### 📦 Produtos
| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `POST` | `/produtos` | Cadastra um novo produto |
| `GET` | `/produtos` | Lista todos os produtos |
| `GET` | `/produtos/{id}` | Busca um produto específico pelo ID |
| `DELETE` | `/produtos/{id}` | Remove um produto do sistema |

### 🛒 Pedidos
| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `POST` | `/pedidos` | Registra um novo pedido |
| `GET` | `/pedidos` | Lista todos os pedidos realizados |
| `GET` | `/pedidos/{id}` | Busca um pedido específico pelo ID |
| `DELETE` | `/pedidos/{id}` | Remove um pedido do sistema |

---

## 👨‍💻 Autor

Desenvolvido por **Rafael Alves de Jesus** 
*   **RU:** 5191069
*   **Curso:** Desenvolvimento Web Back-End - UNINTER
*   **GitHub:** [@rafqel](https://github.com/rafqel)

---
*Este projeto tem fins estritamente acadêmicos.*
