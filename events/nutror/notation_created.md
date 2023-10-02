# Aluno criou uma anotação

## Exemplo

```json
{
    "id": "lnzj8tmh47nblaxdbr8y0vdh",
    "event": "nutror.notation_created",
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
            "hash": "656c71c4b848dfa44666d2893c3438985bbf0085",
            "title": "Título do Curso"
        },
        "lesson": {
            "id": "2108",
            "title": "Título da Aula"
        },
        "createdAt": "2023-09-28T18:12:34Z"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (notation_created)   |
| data.course.hash      | string | Hash identificador do curso         |
| data.course.title     | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |
| data.lesson.id        | string | Id da aula atual                    |
| data.lesson.title     | string | Nome da aula atual                  |