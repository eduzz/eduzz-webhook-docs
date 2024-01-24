# Ingresso ou lote do evento foi alterado

## Exemplo

```json
{
  "id": "b07a59be974e47d192bd9e1951daea47",
  "event": "blinket.ticket_edited",
  "sentDate": "2024-01-20T15:00:00.000Z",
  "data": {
    "producer": {
      "id": "1234",
      "name": "QA Blinket",
      "email": "qa-blinket@eduzz.com"
    },
    "event": {
      "id": "9b056848-beb0-44ff-9e76-d3ac131b6f50",
      "name": "Teste evento",
      "type": "online"
    },
    "tickets": [
      {
        "name": "Padrão",
        "showOnEventPage": true,
        "isPaid": true,
        "isUnlimited": false,
        "buyLimit": 0,
        "buyMinimum": 0
      }
    ],
    "batches": [
      {
        "contentId": "1733797",
        "name": "Lote 1",
        "quantity": 100,
        "startSalesAt": "2024-01-09T15:00:00.000Z",
        "endSalesAt": "2024-01-19T15:00:00.000Z",
        "price": {
          "currency": "BRL",
          "value": 10
        }
      }
    ],
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                           | Tipo    | Descrição                             |
| ------------------------------- | ------- | ------------------------------------- |
| id                              | string  | Id do evento                          |
| event                           | string  | Nome do evento (ticket_edited)        |
| sentDate                        | string  | Data do envio do evento               |
| data.producer.id                | string  | Id do produtor do evento              |
| data.producer.name              | string  | Nome do produtor do evento            |
| data.producer.email             | string  | Email do produtor do evento           |
| data.event.id                   | string  | Id do evento                          |
| data.event.name                 | string  | Nome do evento                        |
| data.event.type                 | string  | Tipo do evento                        |
| data.tickets[0].name            | string  | Nome do ingresso                      |
| data.tickets[0].showOnEventPage | boolean | Mostrar ingresso na página do evento  |
| data.tickets[0].isPaid          | boolean | Ingresso é pago                       |
| data.tickets[0].isUnlimited     | boolean | Ingresso é ilimitado                  |
| data.tickets[0].buyLimit        | number  | Limite de ingressos por compra        |
| data.tickets[0].buyMinimum      | number  | Compra mínima de ingressos por compra |
| data.batches[0].contentId       | string  | Id do conteúdo referente ao lote      |
| data.batches[0].name            | boolean | Nome do lote                          |
| data.batches[0].quantity        | boolean | Quantidade de ingressos do lote       |
| data.batches[0].startSalesAt    | string  | Data de início de vendas do lote      |
| data.batches[0].endSalesAt      | string  | Data de final de vendas do lote       |
| data.batches[0].price.currency  | string  | Moeda do lote                         |
| data.batches[0].price.value     | string  | Preço do lote                         |
| data.createdAt                  | string  | Data de criação do webhook            |
