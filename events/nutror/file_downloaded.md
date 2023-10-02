# Aluno fez download de um arquivo

## Exemplo

```json
{
    "id": "r5r6g31noajle2nkf0xab0uf",
    "event": "nutror.file_downloaded",
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
        "createdAt": "2023-09-25T19:04:09Z"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (file_downloaded)    |
| data.course.hash      | string | Hash identificador do curso         |
| data.course.title     | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.producer.eduzzId | string | Id do produtor no MyEduzz           |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |
| data.lesson.id        | string | Id da aula atual                    |
| data.lesson.title     | string | Nome da aula atual                  |