# Fatura é paga, e as comissões são processadas.

## Exemplo

```json
{
  "id": "g90wu09uwge",
  "event": "myeduzz.commission_processed",
  "sentDate": "2024-01-09T14:45:00.000Z",
  "data": {
    "invoiceId": "12345678",
    "createdAt": "2024-01-09T14:45:00.000Z",
    "price": {
      "currency": "BRL",
      "value": 301.5
    },
    "commissions": {
      "producer": {
        "id": "789451",
        "name": "Producer name",
        "commission": {
          "currency": "BRL",
          "value": 90.0
        }
      },
      "coproducers": [
        {
          "id": "789451",
          "name": "Coproducer name",
          "commission": {
            "currency": "BRL",
            "value": 10.0
          }
        }
      ],
      "affiliates": [
        {
          "id": "658932",
          "name": "Affiliate name",
          "commission": {
            "currency": "BRL",
            "value": 20.0
          }
        }
      ]
    }
  }
}
```

| Campo                                               | Tipo   | Descrição                          |
| --------------------------------------------------- | ------ | ---------------------------------- |
| id                                                  | string | ID do evento                       |
| event                                               | string | Nome do evento                     |
| sentDate                                            | string | Data de envio do evento            |
| data.invoiceId                                      | string | ID da fatura associada             |
| data.createdAt                                      | string | Data de criação de comissionamento |
| data.price.currency                                 | string | Moeda do valor total               |
| data.price.value                                    | number | Valor total da da fatura           |
| data.commissions.producer.id                        | string | ID do produtor                     |
| data.commissions.producer.name                      | string | Nome do produtor                   |
| data.commissions.producer.commission.currency       | string | Moeda da comissão do produtor      |
| data.commissions.producer.commission.value          | number | Valor da comissão do produtor      |
| data.commissions.coproducers[0].id                  | string | ID do coprodutor                   |
| data.commissions.coproducers[0].name                | string | Nome do coprodutor                 |
| data.commissions.coproducers[0].commission.currency | string | Moeda da comissão do coprodutor    |
| data.commissions.coproducers[0].commission.value    | number | Valor da comissão do coprodutor    |
| data.commissions.affiliates[0].id                   | string | ID do afiliado                     |
| data.commissions.affiliates[0].name                 | string | Nome do afiliado                   |
| data.commissions.affiliates[0].commission.currency  | string | Moeda da comissão do afiliado      |
| data.commissions.affiliates[0].commission.value     | number | Valor da comissão do afiliado      |
