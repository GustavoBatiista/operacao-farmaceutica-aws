## Documentação Técnica das APIs

### Visão Geral

Este documento descreve os endpoints disponibilizados pelo sistema de operação farmacêutica.  
A documentação apresenta apenas o contrato de comunicação da API, sem abordar detalhes de implementação interna.

---

### Criar Pedido de Medicamentos

**Endpoint:**  
`POST /pedidos`
 
Registra um novo pedido de medicamentos realizado por uma farmácia parceira junto ao hub farmacêutico.

---

#### Request (Exemplo)

```json
{
  "farmaciaId": "FARM123",
  "itens": [
    {
      "produtoId": "DIPIRONA500",
      "descricao": "Dipirona 500mg",
      "quantidade": 10
    },
    {
      "produtoId": "AMOX500",
      "descricao": "Amoxicilina 500mg",
      "quantidade": 5
    }
  ]
}

---

#### Response (Sucesso)

  {
  "pedidoId": "PED789",
  "status": "CRIADO",
  "valorTotal": 320.50,
  "dataPedido": "2026-01-19"
}


### Consultar Pedido

**Endpoint:**

GET /pedidos/{pedidoId}

Permite que a farmácia parceira consulte o status de um pedido já realizado.

####Request (Exemplo)

GET /pedidos/PED789

####Response

{
  "pedidoId": "PED789",
  "farmaciaId": "FARM123",
  "status": "EM_PROCESSAMENTO",
  "valorTotal": 320.50,
  "previsaoEntrega": "2026-01-22"
}

### Consultar Catálogo de Produtos

**Endpoint:**

GET /produtos

Permite que a farmácia parceira consulte o status de um pedido já realizado.

####Response

  [
  {
    "produtoId": "DIPIRONA500",
    "descricao": "Dipirona 500mg",
    "precoUnitario": 12.50,
    "estoqueDisponivel": 500
  },
  {
    "produtoId": "AMOX500",
    "descricao": "Amoxicilina 500mg",
    "precoUnitario": 22.90,
    "estoqueDisponivel": 200
  }
]

### Consultar Documentos Fiscais do Pedido

**Endpoint:**

GET /pedidos/{pedidoId}/documentos

Permite que a farmácia parceira consulte e realize o download da nota fiscal eletrônica (NF-e) associada a um pedido.

####Response
  
{
  "pedidoId": "PED789",
  "notaFiscalUrl": "https://s3.amazonaws.com/operacao-farmaceutica/nfes/PED789.xml"
}

  
