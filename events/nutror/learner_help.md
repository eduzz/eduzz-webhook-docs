# Aluno solicitou ajuda para o produtor

## Exemplo

```json
{
    "id": "r5r6g31noajle2nkf0xab0uf",
    "event": "nutror.learner_help",
    "data": {
        "producer": {
            "email": "fulano@eduzz.com",
            "name": "Fulano da Silva"
        },
        "learner": {
            "email": "learner@eduzz.com",
            "name": "Ciclano da Silva"
        },
        "course": {
            "hash": "4bba1d18c02755a13ee97521ae61958c3cf9e665",
            "title": "Título do Curso"
        },
        "createdAt": "2023-09-25 19:05:43"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                    | Tipo   | Descrição                           |
|--------------------------|--------|-------------------------------------|
| id                       | string | Id do evento                        |
| event                    | string | Nome do evento (learner_help)       |
| sentDate                 | string | Data do envio                       |
| data.createdAt           | string | Data da criação do evento           |
| data.course.hash         | string | Hash identificador do curso         |
| data.course.title        | string | Nome do curso                       |
| data.producer.email      | string | Email do produtor                   |
| data.producer.name       | string | Nome do produtor                    |
| data.learner.email       | string | Email do aluno                      |
| data.learner.name        | string | Nome do aluno                       |