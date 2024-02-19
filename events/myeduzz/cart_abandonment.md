# Cliente acessa o checkout, preenche os dados básicos, mas não finaliza a compra.

## Exemplo

```json
{
  "id": "g90wu09uwge",
  "event": "myeduzz.cart_abandonment",
  "sentDate": "2024-01-09T14:45:00.000Z",
  "data": {
    "status": "abandoned",
    "buyer": {
      "name": "Alice Johnson",
      "email": "alice.johnson@example.com",
      "phone": "555-789-1234"
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
    ],
    "tracker": {
      "utmMedium": "medium_xzy",
      "utmSource": "facebook",
      "utmCampaign": "campaign_xyz",
      "utmContent": "utm_content"
    }
  }
}
```

| Campo                        | Tipo   | Descrição                                  |
| ---------------------------- | ------ | ------------------------------------------ |
| id                           | string | ID do evento                               |
| event                        | string | Nome do evento                             |
| sentDate                     | string | Data de envio do evento                    |
| data.status                  | string | Status do carrinho                         |
| data.buyer.name              | string | Nome do comprador                          |
| data.buyer.email             | string | Email do comprador                         |
| data.buyer.phone             | string | Telefone do comprador                      |
| data.createdAt               | string | Data de criação do evento                  |
| data.price.currency          | string | Moeda do valor total do carrinho           |
| data.price.value             | number | Valor total do carrinho                    |
| data.items[0].productId      | string | ID do produto no carrinho                  |
| data.items[0].name           | string | Nome do produto no carrinho                |
| data.items[0].price.currency | string | Moeda do preço do produto                  |
| data.items[0].price.value    | number | Preço do produto no carrinho               |
| data.tracker.utmMedium       | string | Valor registrado do parâmetro utm_medium   |
| data.tracker.utmSource       | string | Valor registrado do parâmetro utm_source   |
| data.tracker.utmCampaign     | string | Valor registrado do parâmetro utm_campaign |
| data.tracker.utmContent      | string | Valor registrado do parâmetro utm_content  |
