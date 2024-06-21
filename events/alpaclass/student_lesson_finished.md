# Aluno marcou a aula como concluída

## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_lesson_finished", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
        "email": "teste@email.com",
      },
      "lesson": {
        "id": "38743",
        "name": "teste de aula com link",
      },
      "module": {
        "id": "440",
        "name": "Módulo 1"
      },
      "course": {
        "id": "162",
        "name": "Day trade para iniciantes"
      },
      "team": {
        "id": "538",
        "name": "Escola de Teste"
      },
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                         | 
|---------------------------|--------|---------------------------------------------------| 
| id                        | string | Id do evento                                      | 
| event                     | string | Nome do evento (student_lesson_finished)          | 
| sentDate                  | string | Data do envio do evento                           |
| data.student.id           | string | Id do aluno na escola                             | 
| data.student.name         | string | Nome do aluno                                     |
| data.student.email        | string | Nome do aluno                                     |
| data.lesson.id            | string | Id da aula                                        | 
| data.lesson.name          | string | Nome da aula                                      | 
| data.module.id            | string | Id do módulo                                      | 
| data.module.name          | string | Nome do módulo                                    | 
| data.course.id            | string | Id do curso                                       | 
| data.course.name          | string | Nome do curso                                     |
| data.team.id              | string | Id da escola                                      | 
| data.team.name            | string | Nome da escola                                    | 

