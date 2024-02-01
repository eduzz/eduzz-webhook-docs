# Participante acessou a tela de impressão de ingresso

## Exemplo

```json
{
  "id": "c801061d7d3d4ee5bbb3744a60d88e96",
  "event": "blinket.attendances_printed",
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
    "participants": [
      {
        "inviteKey": "17337976",
        "name": "Teste QA Eduzz",
        "email": "testeeduzzqa@eduzz.com",
        "phone": "+5515999999999",
        "document": {
          "type": "cpf",
          "number": "99999999999"
        },
        "status": "paid",
        "assigned": true,
        "manuallyCreated": false,
        "checkInAt": "2024-01-09T14:25:31.098Z",
        "checkInLink": "https://blinket.testzz.ninja/confirm/9b0f22c4-94fe-4a47-859a-f48987293d38"
      }
    ],
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                                | Tipo   | Descrição                           |
| ------------------------------------ | ------ | ----------------------------------- |
| id                                   | string | Id do evento                        |
| event                                | string | Nome do evento (attendance_printed) |
| sentDate                             | string | Data do envio do evento             |
| data.producer.id                     | string | Id do produtor do evento            |
| data.producer.name                   | string | Nome do produtor do evento          |
| data.producer.email                  | string | Email do produtor do evento         |
| data.event.id                        | string | Id do evento                        |
| data.event.name                      | string | Nome do evento                      |
| data.event.type                      | string | Tipo do evento                      |
| data.participants[0].inviteKey       | string | Número do ingresso                  |
| data.participants[0].name            | string | Nome do participante                |
| data.participants[0].email           | string | Email do participante               |
| data.participants[0].phone           | string | Telefone do participante            |
| data.participants[0].document.type   | string | Tipo de documento do participante   |
| data.participants[0].document.number | string | Número do documento do participante |
| data.participants[0].status          | string | Status do ingresso                  |
| data.participants[0].assigned        | string | Ingresso está atribuído             |
| data.participants[0].manuallyCreated | string | Ingresso foi criado manualmente     |
| data.participants[0].checkInAt       | string | Data que o checkin foi realizado    |
| data.participants[0].checkInLink     | string | Link para o checkin                 |
| data.createdAt                       | string | Data de criação do webhook          |
