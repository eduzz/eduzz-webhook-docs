# Etiquetas dos ingressos foram geradas

## Exemplo

```json
{
  "id": "c801061d7d3d4ee5bbb3744a60d88e96",
  "event": "blinket.attendance_printed",
  "sentDate": "2024-01-20T15:00:00.000Z",
  "data": {
    "producer": {
      "id": "1234",
      "name": "QA Blinket",
      "email": "qa-blinket@eduzz.com"
    },
    "event": {
      "id": "9b056848-beb0-44ff-9e76-d3ac131b6f50",
      "name": "Teste evento atualizacao titulo",
      "type": "online"
    },
    "participants": [
      {
        "name": "Teste QA Eduzz",
        "batchName": "Pago",
        "checkInLink": "https://blinket.testzz.ninja/confirm/9b0f22c4-94fe-4a47-859a-f48987293d38"
      }
    ],
    "createdAt": "2024-01-20T15:00:00.000Z"
  }
}
```

| Campo                            | Tipo   | Descrição                           |
| -------------------------------- | ------ | ----------------------------------- |
| id                               | string | Id do evento                        |
| event                            | string | Nome do evento (attendance_printed) |
| sentDate                         | string | Data do envio do evento             |
| data.producer.id                 | string | Id do produtor do evento            |
| data.producer.name               | string | Nome do produtor do evento          |
| data.producer.email              | string | Email do produtor do evento         |
| data.event.id                    | string | Id do evento                        |
| data.event.name                  | string | Nome do evento                      |
| data.event.type                  | string | Tipo do evento                      |
| data.participants[0].name        | string | Nome do participante                |
| data.participants[0].batchName   | string | Nome do lote                        |
| data.participants[0].checkInLink | string | Link para o checkin                 |
| data.createdAt                   | string | Data de criação do webhook          |
