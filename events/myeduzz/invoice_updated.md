# Fatura é atualizada, como por exemplo, de aberta para paga.

## Exemplo

### Os status para esse evento são: paid, canceled, refunded, analysing, expired, recovering, trial, refused, overdue, scheduled, negociated, readjusted

```json
{
  "id": "g90wu09uwge",
  "event": "myeduzz.invoice_updated",
  "sentDate": "2024-01-09T14:45:00.000Z",
  "data": {
    "id": "12345678",
    "status": "paid",
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
| Campo                                 | Tipo    | Descrição                               |
| ------------------------------------- | ------- | --------------------------------------- |
| id                                    | string  | ID do evento                            |
| event                                 | string  | Nome do evento                          |
| sentDate                              | string  | Data de envio do evento                 |
| data.id                               | string  | ID da transação                         |
| data.status                           | string  | Status da transação                     |
| data.buyer.name                       | string  | Nome do comprador                       |
| data.buyer.email                      | string  | Email do comprador                      |
| data.buyer.phone                      | string  | Telefone do comprador                   |
| data.buyer.phone2                     | string  | Segundo telefone do comprador           |
| data.buyer.cellphone                  | string  | Celular do comprador                    |
| data.createdAt                        | string  | Data de criação da transação            |
| data.price.currency                   | string  | Moeda do valor total da transação       |
| data.price.value                      | number  | Valor total da transação                |
| data.paymentMethod                    | string  | Método de pagamento                     |
| data.installments                     | number  | Número de parcelas                      |
| data.items.productId                  | string  | ID do produto                           |
| data.items.name                       | string  | Nome do produto                         |
| data.items.refundPeriod.durationType  | string  | Tipo de duração do período de reembolso |
| data.items.refundPeriod.value         | number  | Valor do período de reembolso em dias   |
| data.items.price.currency             | string  | Moeda do preço do produto               |
| data.items.price.value                | number  | Preço do produto                        |

