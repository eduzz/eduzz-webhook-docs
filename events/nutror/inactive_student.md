# Aluno inativo

## Exemplo

```json
{
    "id": "r5r6g31noajle2nkf0xab0uf",
    "event": "nutror.inactive_student",
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
            "hash": "6292dab858e745ebc91ba6753619f52ba2502cfc",
            "title": "Título do Curso",
            "inactiveDays": 30
        },
        "createdAt": "2023-09-13 21:00:36"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                    | Tipo   | Descrição                           |
|--------------------------|--------|-------------------------------------|
| id                       | string | Id do evento                        |
| event                    | string | Nome do evento (inactive_student)   |
| sentDate                 | string | Data do envio                       |
| data.createdAt           | string | Data da criação do evento           |
| data.course.hash         | string | Hash identificador do curso         |
| data.course.title        | string | Nome do curso                       |
| data.course.inactiveDays | string | Nome do curso                       |
| data.producer.email      | string | Email do produtor                   |
| data.producer.name       | string | Nome do produtor                    |
| data.learner.email       | string | Email do aluno                      |
| data.learner.name        | string | Nome do aluno                       |