# Fatura é criada e está aguardando pagamento.

## Exemplo

```json
{
  "id": "g90wu09uwge",
  "event": "myeduzz.invoice_opened",
  "sentDate": "2024-01-09T14:45:00.000Z",
  "data": {
    "id": "12345678",
    "status": "open",
    "buyer": {
      "name": "Alice Johnson",
      "email": "alice.johnson@example.com",
      "phone": "555-789-1234",
      "phone2": "555-987-6543",
      "cellphone": "555-321-9876"
    },
    "producer": {
      "email": "fulano@eduzz.com",
      "name": "Fulano da Silva",
      "id": "123456"
    },
    "createdAt": "2024-01-09T14:45:00.000Z",
    "price": {
      "currency": "BRL",
      "value": 301.5
    },
    "utm": {
      "source": "abc",
      "campaign": "def",
      "content": "ghi",
      "medium": "jkl"
    },
    "installments": 1,
    "items": [
      {
        "productId": "P567",
        "name": "Widget X",
        "price": {
          "currency": "BRL",
          "value": 150.75
        }
      },
      {
        "productId": "P789",
        "name": "Gadget Y",
        "price": {
          "currency": "BRL",
          "value": 150.75
        }
      }
    ]
  }
}
```

| Campo                        | Tipo   | Descrição                        |
| ---------------------------- | ------ | -------------------------------- |
| id                           | string | ID do evento                     |
| event                        | string | Nome do evento                   |
| sentDate                     | string | Data de envio do evento          |
| data.id                      | string | ID da fatura                     |
| data.status                  | string | Status da fatura                 |
| data.buyer.name              | string | Nome do comprador                |
| data.buyer.email             | string | Email do comprador               |
| data.buyer.phone             | string | Telefone do comprador            |
| data.buyer.phone2            | string | Segundo telefone do comprador    |
| data.buyer.cellphone         | string | Celular do comprador             |
| data.producer.name           | string | Nome do produtor                 |
| data.procer.email            | string | Email do produtor                |
| data.procer.id               | string | ID do produtor                   |
| data.createdAt               | string | Data de criação da fatura        |
| data.price.currency          | string | Moeda do valor total da fatura   |
| data.price.value             | number | Valor total da fatura            |
| data.installments            | number | Número de parcelas               |
| data.utm.source              | string | Origem do tráfego fonte da venda |
| data.utm.campaign            | string | Nome da campanha fonte da venda  |
| data.utm.medium              | string | Mídia fonte da venda             |
| data.utm.content             | string | Conteúdo relacionado à venda     |
| data.items[0].productId      | string | ID do produto                    |
| data.items[0].name           | string | Nome do produto                  |
| data.items[0].price.currency | string | Moeda do preço do produto        |
| data.items[0].price.value    | number | Preço do produto                 |
