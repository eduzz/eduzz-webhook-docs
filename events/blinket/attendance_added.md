# Participante foi adicionado ao evento

## Exemplo

```json
{
  "id": "33cad82ae0d84a66b139f521e1c62e29",
  "event": "blinket.attendance_added",
  "sentDate": "2024-01-20T15:00:00.000Z",
  "data": {
    "producer": {
      "id": "1234",
      "name": "João Silva",
      "email": "joaosilva@teste.com"
    },
    "event": {
      "id": "9b056848-beb0-44ff-9e76-d3ac131b6f50",
      "name": "Teste evento",
      "type": "online"
    },
    "ticket": {
      "name": "Padrão",
      "isPaid": true
    },
    "batch": {
      "contentId": "1733797",
      "name": "Lote 1",
      "price": {
        "currency": "BRL",
        "value": 10.0
      }
    },
    "buyer": {
      "name": "Maria Silva",
      "email": "mariasilva@teste.com",
      "phone": "+5515999999999",
      "id": "123123"
    },
    "participant": {
      "inviteKey": "99999999",
      "name": "Maria Silva",
      "email": "mariasilva@teste.com",
      "phone": "+5515999999999",
      "document": {
        "type": "cpf",
        "number": "99999999999"
      },
      "status": "paid",
      "assigned": false,
      "manuallyCreated": false,
      "checkInAt": null,
      "checkInLink": "https://blinket/confirm/hashuuid"
    },
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                            | Tipo    | Descrição                           |
| -------------------------------- | ------- | ----------------------------------- |
| id                               | string  | Id do evento                        |
| event                            | string  | Nome do evento (attendance_added)   |
| sentDate                         | string  | Data do envio do evento             |
| data.producer.id                 | string  | Id do produtor do evento            |
| data.producer.name               | string  | Nome do produtor do evento          |
| data.producer.email              | string  | Email do produtor do evento         |
| data.event.id                    | string  | Id do evento                        |
| data.event.name                  | string  | Nome do evento                      |
| data.event.type                  | string  | Tipo do evento                      |
| data.ticket.name                 | string  | Nome do ingresso                    |
| data.ticket.isPaid               | boolean | Ingresso é pago                     |
| data.batch.contentId             | string  | Id do conteúdo referente ao lote    |
| data.batch.name                  | string  | Nome do lote                        |
| data.batch.price.currency        | string  | Moeda do lote                       |
| data.batch.value                 | number  | Preço do lote                       |
| data.buyer.name                  | string  | Nome do comprador                   |
| data.buyer.email                 | string  | Email do comprador                  |
| data.buyer.phone                 | string  | Telefone do comprador               |
| data.buyer.id                    | string  | Id do comprador na Eduzz            |
| data.participant.inviteKey       | string  | Número do ingresso                  |
| data.participant.name            | string  | Nome do participante                |
| data.participant.email           | string  | Email do participante               |
| data.participant.phone           | string  | Telefone do participante            |
| data.participant.document.type   | string  | Tipo de documento do participante   |
| data.participant.document.number | string  | Número do documento do participante |
| data.participant.status          | string  | Status do ingresso                  |
| data.participant.assigned        | boolean | Ingresso está atribuído             |
| data.participant.manuallyCreated | boolean | Ingresso foi criado manualmente     |
| data.participant.checkInAt       | string  | Data que o checkin foi realizado    |
| data.participant.checkInLink     | string  | Link para o checkin                 |
| data.createdAt                   | string  | Data de criação do webhook          |
