# Aluno concluiu o curso
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_course_finished", 
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
| event                     | string | Nome do evento (student_course_finished)    | 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.student.email        | string | E-mail do aluno                             |
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               | 
| data.team.id              | string | Id da escola                                | 
| data.team.name            | string | Nome da escola                              | 

# Aluno concluiu o curso
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_completed_course", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
      },
      "course": { 
        "id": "68", 
        "name": "Day trade para iniciantes", 
        "finishedAt": "2024-06-12T12:00:10.000Z", 
      },
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                   | 
|---------------------------|--------|---------------------------------------------| 
| id                        | string | Id do evento                                | 
| event                     | string | Nome do evento (student_completed_course)   | 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               | 
| data.course.finishedAt    | string | Data que o aluno concluiu o curso           | 

