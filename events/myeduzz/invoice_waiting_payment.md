# Fatura é atualizada para aguardando pagamento.

## Exemplo

```json
{
  "id": "g90wu09uwge",
  "event": "myeduzz.invoice_waiting_payment",
  "sentDate": "2024-01-09T14:45:00.000Z",
  "data": {
    "id": "12345678",
    "status": "waiting_payment",
    "producer": {
      "id": "123456"
      "email": "fulano@eduzz.com",
      "name": "Fulano da Silva",
    },
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
    "paymentMethod": "creditCard",
    "installments": 1,
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
  }
}
```

| Campo                                   | Tipo   | Descrição                               |
| --------------------------------------- | ------ | --------------------------------------- |
| id                                      | string | ID do evento                            |
| event                                   | string | Nome do evento                          |
| sentDate                                | string | Data de envio do evento                 |
| data.id                                 | string | ID da fatura                            |
| data.status                             | string | Status da fatura                        |
| data.buyer.name                         | string | Nome do comprador                       |
| data.buyer.email                        | string | Email do comprador                      |
| data.buyer.phone                        | string | Telefone do comprador                   |
| data.buyer.phone2                       | string | Segundo telefone do comprador           |
| data.buyer.cellphone                    | string | Celular do comprador                    |
| data.createdAt                          | string | Data de criação fatura                  |
| data.price.currency                     | string | Moeda do valor total da fatura          |
| data.price.value                        | number | Valor total da fatura                   |
| data.installments                       | number | Número de parcelas                      |
| data.paymentMethod                      | string | Método de pagamento                     |
| data.producer.id                        | string | ID do produtor                          |
| data.producer.name                      | string | Nome do produtor                        |
| data.producer.email                     | string | Email do produtor                       |
| data.items[0].productId                 | string | ID do produto                           |
| data.items[0].name                      | string | Nome do produto                         |
| data.items[0].refundPeriod.durationType | string | Tipo de duração do período de reembolso |
| data.items[0].refundPeriod.value        | number | Valor do período de reembolso em dias   |
| data.items[0].price.currency            | string | Moeda do preço do produto               |
| data.items[0].price.value               | number | Preço do produto                        |
