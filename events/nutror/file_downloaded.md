# Aluno fez download de um arquivo

## Exemplo

```json
{
    "id": "r5r6g31noajle2nkf0xab0uf",
    "event": "nutror.file_downloaded",
    "data": {
        "lesson": {
            "id": "zra8ahwim3tj96y0m83jcddo",
            "title": "Parte 1 - Ingredientes",
        },
        "courses": [
            {
                "hash": "u1rw9gdgagfp0za0mn4rfhuh",
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