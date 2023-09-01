# Aluno completou 75% da aula

## Exemplo

```json
{
    "id": "p8djscz8lg5k76avlyihkudy",
    "event": "nutror.complete_lesson_75",
    "data": {
        "courses": [
            {
                "hash": "up0e6q9iyrd6mpcw74js5i71",
                "title": "Como se tornar padeiro"
            }
        ],
        "producer": {
            "email": "seu-email@host.com",
            "name": "Seu Nome",
            "eduzzId": 91823745
        },
        "learner": {
            "email": "email-aluno@host.com",
            "name": "Nome do aluno"
        },
        "createdAt": "2023-08-31T18:34:23.023Z",
        "content": {
            "progress": 75
        }
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (certificate_viewed) |
| data.courses.0.hash   | string | Hash identificador do curso         |
| data.courses.0.title  | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.producer.eduzzId | string | Id do produtor no MyEduzz           |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |
| data.content.progress | number | Percentual de progresso atual       |