# Aula salva

## Exemplo

```json
{
    "id": "lnzj8tmh47nblaxdbr8y0vdh",
    "event": "nutror.lesson_saved",
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
        "lesson": {
            "id": "3865",
            "title": "Título da Aula"
        },
        "createdAt": "2023-09-25T19:02:28Z",
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (lesson_saved)       |
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