📋 Sobre o Projeto
API de e-commerce desenvolvida com Spring Boot para gerenciamento de produtos, pedidos e usuários.

🚀 Tecnologias Utilizadas
Java 21
Spring Boot 3.1.0
Spring Data JPA
MySQL 8.0
Maven

🛠️ Funcionalidades
✅ Cadastro de usuários
🛒 Gerenciamento de produtos
📦 Controle de pedidos
🔐 Autenticação de usuários
📝 Endpoints

Usuários
POST /usuarios - Criar usuário
GET /usuarios - Listar usuários
GET /usuarios/{id} - Buscar usuário por ID

Produtos
POST /produtos - Criar produto
GET /produtos - Listar produtos
GET /produtos/{id} - Buscar produto por ID

Pedidos
POST /pedidos - Criar pedido
GET /pedidos - Listar pedidos
GET /pedidos/{id} - Buscar pedido por ID
PUT /pedidos/{id} - Atualizar pedido
DELETE /pedidos/{id} - Deletar pedido
GET /pedidos/cliente/{clienteId} - Listar pedidos do cliente
GET /pedidos/{id}/itens - Listar itens do pedido

🎨 Exemplos de Requisições
Criar Usuário
{
    "nome": "lucas Silva",
    "email": "lucas@email.com",
    "telefone": "11999999999",
    "senha": "123456"
}
Criar Produto
{
    "nome": "Smartphone XeZ",
    "descricao": "Smartphone de última geração",
    "preco": 1999.99,
    "imagemUrl": "https://exemplo.com/smartphone.jpg"
}
Criar Pedido
{
    "cliente": {
        "id": 1
    },
    "items": [
        {
            "produtoId": 1,
            "quantidade": 2,
            "preco": 1999.99
        }
    ]
}

🚀 Como Executar
Clone o repositório "https://github.com/lucasdev077/Ecommerce-lucas/new/main"
Configure o banco de dados no `application.properties`
Execute o projeto, mas ligue no banco do Workbench
