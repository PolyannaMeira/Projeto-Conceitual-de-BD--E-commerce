# 📦 E-commerce Database Schema

## 📝 Descrição
Este projeto apresenta um modelo conceitual de banco de dados para um sistema de e-commerce, estruturado para gerenciar produtos, pedidos, clientes, formas de pagamento, estoque e entregas. O design prioriza a integridade dos dados, a segurança das informações sensíveis e a eficiência na gestão de pedidos e transações.

---

## 🛠️ Modelagem do Banco de Dados
O esquema do banco de dados é composto pelas seguintes entidades:

### 🔹 **Cliente**
- Armazena informações pessoais dos clientes, como nome, e-mail e endereço.

### 🔹 **Pedido**
- Representa os pedidos realizados pelos clientes.
- Relacionado com a entidade Cliente.
- Conectado à entidade Entrega.

### 🔹 **Entrega**
- Controla o status da entrega dos pedidos.
- Relacionado com a entidade Pedido.
- Possui informações como código de rastreio e data prevista de entrega.

### 🔹 **Produto**
- Representa os produtos disponíveis na loja.
- Relacionado com estoque e fornecedores.

### 🔹 **Estoque**
- Gerencia a quantidade de produtos disponíveis.
- Relacionado com produtos e fornecedores.

### 🔹 **Fornecedor**
- Armazena informações sobre fornecedores dos produtos.
- Relacionado com o controle de estoque.

### 🔹 **Formas de Pagamento**
- Controla os métodos de pagamento.
- **Importante:** Não armazenamos o código de segurança (CVV) dos cartões, apenas um token de transação para fins de conformidade com normas de segurança (ex.: PCI-DSS).

### 🔹 **Relação Produto/Pedido**
- Define os produtos associados a cada pedido.
- Garante que um pedido possa conter vários produtos.

---

## 🚀 Como Utilizar
1. Clone este repositório:
   ```bash
   git clone https://github.com/PolyannaMeira/Projeto-Conceitual-de-BD--E-commerce.git
   ```
2. Importe o esquema SQL no seu banco de dados preferido.
3. Teste as consultas e relações entre as tabelas.

---

## 📌 Tecnologias Utilizadas
- 
- **MySql Workbench** para representação visual da estrutura do banco.

---

## 📧 Contato
Caso tenha dúvidas ou sugestões, fique à vontade para abrir uma issue ou entrar em contato!

---

### 📜 Licença
Este projeto está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

