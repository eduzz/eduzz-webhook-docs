# Aluno acessou a comunidade

## Exemplo

```json
{
    "id": "sp18cyp4dghx8irfss4w8uvi",
    "event": "nutror.community_viewed",
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
        "createdAt": "2023-09-28T18:29:03Z"
    },
    "sentDate": "2023-08-31T18:34:23.023Z"
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|
| id                    | string | Id do evento                        |
| event                 | string | Nome do evento (community_viewed)   |
| sentDate              | string | Data do envio                       |
| data.createdAt        | string | Data da criação do evento           |
| data.courses.hash     | string | Hash identificador do curso         |
| data.courses.title    | string | Nome do curso                       |
| data.producer.email   | string | Email do produtor                   |
| data.producer.name    | string | Nome do produtor                    |
| data.learner.email    | string | Email do aluno                      |
| data.learner.name     | string | Nome do aluno                       |