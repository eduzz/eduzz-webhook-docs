# Ultimo acesso do aluno no curso
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_course_last_seen_at", 
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
| event                     | string | Nome do evento (student_course_last_seen_at)| 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.student.email        | string | E-mail do aluno                             |
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               | 
| data.team.id              | string | Id da escola                                | 
| data.team.name            | string | Nome da escola                              | 

# Aluno comentou na aula
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_commented_on_lesson", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
      },
      "lesson": { 
        "id": "68", 
        "name": "Aula 1 - Melhores ações do setor de energia", 
      },
      "comment": {
        "body": "Adorei a aula, espero conseguir aplicar os aprendizados!",
        "createdAt": "2024-06-12T12:00:10.000Z", 
      },
      "course": { 
        "id": "25", 
        "name": "Day trade para iniciantes", 
      },
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                   | 
|---------------------------|--------|---------------------------------------------| 
| id                        | string | Id do evento                                | 
| event                     | string | Nome do evento (student_commented_on_lesson)| 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.lesson.id            | string | Id da aula                                  | 
| data.lesson.name          | string | Nome da aula                                | 
| data.comment.body         | string | Conteúdo do comentário                      | 
| data.comment.createdAt    | string | Data da criação do comentário               | 
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               |

