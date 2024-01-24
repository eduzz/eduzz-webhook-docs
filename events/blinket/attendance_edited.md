# Participante teve seus dados alterados

## Exemplo

```json
{
  "id": "ccf4c9664acd42b69c1b48ac513bcdb5",
  "event": "blinket.attendance_edited",
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
    "participant": {
      "inviteKey": "17337976",
      "name": "Teste QA Eduzz",
      "email": "testeeduzzqa@eduzz.com",
      "phone": "+5515999999999",
      "document": {
        "type": "cpf",
        "number": "99999999999"
      },
      "status": "paid",
      "assigned": false,
      "manuallyCreated": false,
      "checkInAt": null
    },
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                            | Tipo    | Descrição                           |
| -------------------------------- | ------- | ----------------------------------- |
| id                               | string  | Id do evento                        |
| event                            | string  | Nome do evento (attendance_edited)  |
| sentDate                         | string  | Data do envio do evento             |
| data.producer.id                 | string  | Id do produtor do evento            |
| data.producer.name               | string  | Nome do produtor do evento          |
| data.producer.email              | string  | Email do produtor do evento         |
| data.event.id                    | string  | Id do evento                        |
| data.event.name                  | string  | Nome do evento                      |
| data.event.type                  | string  | Tipo do evento                      |
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
| data.createdAt                   | string  | Data da criação do evento           |
