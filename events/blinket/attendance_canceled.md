# Ingresso foi cancelado

## Exemplo

```json
{
  "id": "6935513134164a7fac29eb686aec9da7",
  "event": "blinket.attendance_canceled",
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
    "participant": {
      "inviteKey": "99999999",
      "name": "Maria Silva",
      "email": "mariasilva@test.com",
      "phone": "+5599999999999",
      "status": "canceled",
      "manuallyCreated": false
    },
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                            | Tipo    | Descrição                            |
| -------------------------------- | ------- | ------------------------------------ |
| id                               | string  | Id do evento                         |
| event                            | string  | Nome do evento (attendance_canceled) |
| sentDate                         | string  | Data do envio do evento              |
| data.producer.id                 | string  | Id do produtor do evento             |
| data.producer.name               | string  | Nome do produtor do evento           |
| data.producer.email              | string  | Email do produtor do evento          |
| data.event.id                    | string  | Id do evento                         |
| data.event.name                  | string  | Nome do evento                       |
| data.event.type                  | string  | Tipo do evento                       |
| data.participant.inviteKey       | string  | Número do ingresso                   |
| data.participant.name            | string  | Nome do participante                 |
| data.participant.email           | string  | Email do participante                |
| data.participant.phone           | string  | Telefone do participante             |
| data.participant.status          | string  | Status do ingresso                   |
| data.participant.manuallyCreated | boolean | Ingresso foi criado manualmente      |
| data.createdAt                   | string  | Data de criação do webhook           |
