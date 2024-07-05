# Aluno cadastrado na escola

## Exemplo

```json
{
    "id": "4c832x3ynl8dwe7454941xzr5",
    "event": "alpaclass.student_created",
    "sentDate": "2024-06-12T12:00:10.000Z",
    "data": {
      "student": {
        "id": "457391c9c82bfdcbb4947278c0401e41",
        "name": "Fulano da Silva",
        "email": "fulano@eduzz.com",
        "document": "123.456.789-00",
        "phone": "11999999999",
        "createdAt": "2024-06-12T12:00:00.000Z",
        "locale": "pt_BR",
      },
      "team": {
        "id": "457391c9c82bfdcbb4947278c0401e41",
        "name": "Escola Teste",
      },
    }
}
```

## Dados enviados

| Campo                     | Tipo   | Descrição                                        |
|---------------------------|--------|--------------------------------------------------|
| id                        | string | Id do evento                                     |
| event                     | string | Nome do evento (student_created)                 |
| sentDate                  | string | Data do envio do evento                          |
| data.student.id           | string | Id do aluno na escola                            |
| data.student.name         | string | Nome do aluno                                    |
| data.student.email        | string | Email do aluno                                   |
| data.student.document     | string | Documento do aluno. Geralmente é o CPF           |
| data.student.phone        | string | Telefone/Celular do aluno                        |
| data.student.createdAt    | string | Data em que o aluno foi cadastrado na escola     |
| data.student.locale       | string | Idioma do aluno                                  |
| data.team.id              | string | Id da escola                                     |
| data.team.name            | string | Nome da escola                                   |
