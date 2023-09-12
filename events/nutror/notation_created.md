# Aluno criou uma anotação

## Exemplo

```json
{
    "id": "lnzj8tmh47nblaxdbr8y0vdh",
    "event": "nutror.notation_created",
    "data": {
        "lesson": {
            "id": "t35v9qoifjbfbagx7zr37ykh",
            "title": "Parte 1 - Ingredientes",
        },
        "courses": [
            {
                "hash": "jueq2plrng753v5yn1y2r7x5",
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
        "createdAt": "2023-08-31T18:34:23.023Z"
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
| data.lesson.id        | string | Id da aula atual                   |
| data.lesson.title     | string | Nome da aula atual                 |