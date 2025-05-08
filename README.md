# Refinando um Modelo Conceitual de Banco de Dados para E-Commerce
Desafio de Projeto da [Formação SQL Database Specialist](https://www.dio.me/) da [DIO](https://www.dio.me/)

## 📋 Descrição do Desafio

### 🛍️ Contexto do Sistema
Modelagem de banco de dados para um e-commerce com os requisitos:

**Entidades Principais:**
- `Produto` (com controle de estoque)
- `Fornecedor` (relacionamento com produtos)
- `Cliente` (PF/PJ)
- `Pedido` (com status de entrega)

### 📦 Regras de Negócio - Produtos
- Plataforma única com vendedores terceirizados
- Relacionamento 1:N com fornecedores
- Composição em pedidos (1 pedido → N produtos)

### 👥 Regras de Negócio - Clientes
- **Cadastro dual:** CPF (PF) ou CNPJ (PJ)
- **Cálculo de frete** baseado no endereço
- **Política de devoluções:** período de carência
- Histórico de pedidos (1 cliente → N pedidos)

### 📮 Regras de Negócio - Pedidos
- **Atributos obrigatórios:**
  - Dados de compra
  - Endereço de entrega
  - Status (incluindo cancelamento)
- Composição flexível (N produtos por pedido)

## ✅ Solução Proposta
[▶️ Clique para ver a modelagem completa]() | [📁 Arquivo SQL]()


## 🛠️ Tecnologias Utilizadas
- **MySQL Workbench** - Para diagramação do modelo relacional
- **Git/GitHub** - Versionamento e documentação
