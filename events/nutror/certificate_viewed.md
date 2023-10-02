# Aluno acessou o certificado

## Exemplo

```json
{
    "id": "d4neemljy87rv3og472ag6hl",
    "event": "nutror.certificate_viewed",
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
            "hash": "a3cc1883deab35a35dfc4e3dbc9bbc8c65dc5942",
            "title": "Título do Curso"
        },
        "createdAt": "2023-09-06 17:32:14"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (certificate_viewed) |
| data.createdAt        | string | Data da criação do evento           |
| data.course.hash      | string | Hash identificador do curso         |
| data.course.title     | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |
