# Diagrama Modelagem ER para E-commerce

Este repositório contém o diagrama Entidade-Relacionamento (ER) de um sistema de e-commerce, desenvolvido como parte de um exercício prático.

## Descrição do Projeto

O diagrama ER representa a estrutura de um banco de dados para um e-commerce, com foco em:
- **Clientes**: Divisão entre Pessoa Física (PF) e Pessoa Jurídica (PJ).
- **Pagamentos**: Suporte a múltiplas formas de pagamento.
- **Entregas**: Rastreamento de status e código de rastreio.

### Desenvolvimento
1. **Em Aula**:
   - Reproduzi parte do diagrama ER inicial, com as entidades básicas como `cliente`, `produto` e `pedido`.

2. **Como Tarefa**:
   - Refinei o diagrama com as seguintes adições:
     - **Divisão de Clientes**: Criei entidades especializadas para `cliente_pf` (Pessoa Física) e `cliente_pj` (Pessoa Jurídica).
     - **Pagamento**: Adicionei a entidade `pagamento`, permitindo que um cliente cadastre múltiplas formas de pagamento.
     - **Entrega**: Implementei a entidade `entrega`, com status e código de rastreio para acompanhamento.

## Diagrama ER

![Diagrama ER](![Diagrama Modelagem E-commerce](https://github.com/user-attachments/assets/a6b38d40-2650-42f6-98d5-5477a9e0afa8)
)

### Legenda das Cores
- **Tabelas Verdes**: Representam as **entidades principais** do sistema.
- **Tabelas Rosas**: Representam **entidades de relacionamento muitos-para-muitos**.

## Estrutura do Banco de Dados

### Entidades Principais
- **`cliente`**: Armazena informações comuns a todos os clientes.
- **`cliente_pf`**: Detalhes específicos de Pessoa Física (CPF, data de nascimento).
- **`cliente_pj`**: Detalhes específicos de Pessoa Jurídica (CNPJ, razão social).
- **`pagamento`**: Formas de pagamento cadastradas pelos clientes.
- **`entrega`**: Informações de rastreamento e status das entregas.

### Relacionamentos
- Um `cliente` pode ser **PJ** ou **PF**, mas não ambos.
- Um `cliente` pode ter múltiplos `pagamentos`.
- Cada `pedido` está associado a uma `entrega`.

## Contribuições
Este projeto foi desenvolvido como parte de um exercício prático. Contribuições e sugestões são bem-vindas! Sinta-se à vontade para abrir uma **issue** ou enviar um **pull request**.

---

Desenvolvido com por [Elisangela Sena].
