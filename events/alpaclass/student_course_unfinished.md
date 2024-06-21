# Aluno desmarca como concluido o curso
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_course_unfinished", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
        "email": "teste@email.com",
      },
      "course": { 
        "id": "68", 
        "name": "Day trade para iniciantes", 
      },
      "team": { 
        "id": "68", 
        "name": "Escola de teste", 
      },
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                   | 
|---------------------------|--------|---------------------------------------------| 
| id                        | string | Id do evento                                | 
| event                     | string | Nome do evento (student_course_unfinished)  | 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.student.email        | string | E-mail do aluno                             |
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               | 
| data.team.id              | string | Id da escola                                | 
| data.team.name            | string | Nome da escola                              | 

