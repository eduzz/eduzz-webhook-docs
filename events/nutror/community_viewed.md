# Aluno acessou a comunidade

## Exemplo

```json
{
    "id": "sp18cyp4dghx8irfss4w8uvi",
    "event": "nutror.community_viewed",
    "data": {
        "courses": [
            {
                "hash": "sb3cst68q8amfe6cfaby6rqq",
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