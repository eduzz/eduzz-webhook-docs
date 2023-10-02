# Aluno criou novo comentário

## Exemplo

```json
{
    "id": "jurjck13py6winxcgeievcho",
    "event": "nutror.comment_created",
    "data": {
        "producer": {
            "email": "fulano@eduzz.com",
            "name": "Fulano da Silva"
        },
        "learner": {
            "email": "fulano@eduzz.com",
            "name": "Ciclano da Silva"
        },
        "course": {
            "hash": "1feb6e6b27ccaf9edee926908f710808e2d6c7e6",
            "title": "Título do Curso"
        },
        "lesson": {
            "id": "13",
            "title": "Título da Aula"
        },
        "createdAt": "2023-09-26T13:51:15Z"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (comment_created)    |
| sentDate              | string | Data do envio                       |
| data.createdAt        | string | Data da criação do evento           |
| data.course.hash      | string | Hash identificador do curso         |
| data.course.title     | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |
| data.lesson.id        | string | Id da aula atual                    |
| data.lesson.title     | string | Nome da aula atual                  |