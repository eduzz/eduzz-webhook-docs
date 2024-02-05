# Cliente acessa o checkout, preenche os dados básicos, mas não finaliza a compra.

## Exemplo

```json
{
  "data": {
    "status": "abandoned_cart",
    "buyer": {
      "name": "Alice Johnson",
      "email": "alice.johnson@example.com",
      "phone": "555-789-1234",
      "phone2": "555-987-6543",
      "cellphone": "555-321-9876"
    },
    "createdAt": "2024-01-09T14:45:00.000Z",
    "price": {
      "currency": "BRL",
      "value": 301.5
    },
    "items": [
      {
        "productId": "P567",
        "name": "Widget X",
        "refundPeriod": {
          "durationType": "days",
          "value": 7
        },
        "price": {
          "currency": "BRL",
          "value": 150.75
        }
      },
      {
        "productId": "P789",
        "name": "Gadget Y",
        "refundPeriod": {
          "durationType": "days",
          "value": 7
        },
        "price": {
          "currency": "BRL",
          "value": 150.75
        }
      }
    ]
  },
  "metadata": {
    "productId": ["P567", "P789"],
    "userId": "123",
    "email": "alice.johnson@example.com"
  }
}
```

| Campo                        | Tipo   | Descrição                             |
| ---------------------------- | ------ | ------------------------------------- |
| data.status                  | string | Status do carrinho                    |
| data.buyer.name              | string | Nome do comprador                     |
| data.buyer.email             | string | Email do comprador                    |
| data.buyer.phone             | string | Telefone do comprador                 |
| data.buyer.phone2            | string | Segundo telefone do comprador         |
| data.buyer.cellphone         | string | Celular do comprador                  |
| data.createdAt               | string | Data de criação do evento             |
| data.price.currency          | string | Moeda do valor total do carrinho      |
| data.price.value             | number | Valor total do carrinho               |
| data.items.productId         | string | ID do produto no carrinho             |
| data.items.name              | string | Nome do produto no carrinho           |
| data.items.refundPeriod      | object | Período de reembolso do produto       |
| data.items.price.currency    | string | Moeda do preço do produto             |
| data.items.price.value       | number | Preço do produto no carrinho          |
| metadata.productId           | array  | IDs dos produtos no carrinho          |
| metadata.userId              | string | ID do usuário relacionado             |
| metadata.email               | string | Email do usuário relacionado          |
