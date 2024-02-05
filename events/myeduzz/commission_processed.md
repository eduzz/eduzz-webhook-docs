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
        "currency": "BRL",
        "value": 90.0
      },
      "coproducer": [
        {
          "id": "789451",
          "name": "Coproducer name",
          "currency": "BRL",
          "value": 10.0
        }
      ],
      "affiliates": [
        {
          "id": "658932",
          "name": "Affiliate name",
          "currency": "BRL",
          "value": 2.0
        }
      ]
    }
  }
}
```
| Campo                            | Tipo   | Descrição                             |
| -------------------------------- | ------ | ------------------------------------- |
| id                               | string | ID do evento                          |
| event                            | string | Nome do evento                        |
| sentDate                         | string | Data de envio do evento               |
| data.invoiceId                  | string | ID da fatura associada à comissão     |
| data.createdAt                  | string | Data de criação do evento             |
| data.price.currency             | string | Moeda do valor total da comissão      |
| data.price.value                | number | Valor total da comissão               |
| data.commissions.producer.id    | string | ID do produtor da comissão            |
| data.commissions.producer.name  | string | Nome do produtor da comissão          |
| data.commissions.producer.currency | string | Moeda da comissão do produtor       |
| data.commissions.producer.value | number | Valor da comissão do produtor         |
| data.commissions.coproducer     | array  | Lista de coprodutores                 |
| data.commissions.coproducer.id  | string | ID do coprodutor                      |
| data.commissions.coproducer.name| string | Nome do coprodutor                    |
| data.commissions.coproducer.currency | string | Moeda da comissão do coprodutor |
| data.commissions.coproducer.value | number | Valor da comissão do coprodutor       |
| data.commissions.affiliates     | array  | Lista de afiliados                    |
| data.commissions.affiliates.id  | string | ID do afiliado                        |
| data.commissions.affiliates.name| string | Nome do afiliado                      |
| data.commissions.affiliates.currency | string | Moeda da comissão do afiliado    |
| data.commissions.affiliates.value | number | Valor da comissão do afiliado         |
