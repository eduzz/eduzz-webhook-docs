# Nova matrícula

## Exemplo

```json
{
    "id": "lnzj8tmh47nblaxdbr8y0vdh",
    "event": "nutror.enrollment_created",
    "data": {
        "producer": {
            "email": "fulano@eduzz.com",
            "name": "Fulano da Silva"
        },
        "learner": {
            "email": "learner@eduzz.com",
            "name": "Ciclano da Silva"
        },
        "content": {
            "hash": "6b25298f91736fa32da03d986b354c304ee0442d",
            "title": "Teste cache invite"
        },
        "courses": [
            {
                "hash": "6b25298f91736fa32da03d986b354c304ee0442d",
                "title": "Título do Curso"
            }
        ],
        "createdAt": "2023-09-20 17:25:42"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                  | Tipo   | Descrição                           |
|------------------------|--------|-------------------------------------|
| id                     | string | Id do evento                        |
| event                  | string | Nome do evento (enrollment_created) |
| sentDate               | string | Data do envio                       |
| data.createdAt         | string | Data da criação do evento           |
| data.courses.[0].hash  | string | Hash identificador do curso         |
| data.courses.[0].title | string | Nome do curso                       |
| data.producer.email    | string | Email do produtor                   |
| data.producer.name     | string | Nome do produtor                    |
| data.content.hash      | string | Email do produtor                   |
| data.content.title     | string | Email do produtor                   |
| data.learner.email     | string | Email do aluno                      |
| data.learner.name      | string | Nome do aluno                       |