# Aluno comentou na aula
## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_comment_created", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva",
        "email": "teste@email.com",
      },
      "lesson": { 
        "id": "68", 
        "name": "Aula 1 - Melhores ações do setor de energia", 
      },
      "module": { 
        "id": "25", 
        "name": "Módulo 1", 
      },
      "course": { 
        "id": "28", 
        "name": "Day trade para iniciantes", 
      },
      "team": { 
        "id": "58", 
        "name": "Escola de teste", 
      },
      "comment": "Adorei a aula, espero conseguir aplicar os aprendizados!",
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                   | 
|---------------------------|--------|---------------------------------------------| 
| id                        | string | Id do evento                                | 
| event                     | string | Nome do evento (student_comment_created)    | 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | string | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.student.email        | string | E-mail do aluno                             |
| data.lesson.id            | string | Id da aula                                  | 
| data.lesson.name          | string | Nome da aula                                | 
| data.module.id            | string | Id do módulo                                | 
| data.module.name          | string | Nome do módulo                              |
| data.course.id            | string | Id do curso                                 | 
| data.course.name          | string | Nome do curso                               |
| data.team.id              | string | Id da escola                                | 
| data.team.name            | string | Nome da escola                              |
| data.comment              | string | Conteúdo do comentário                      | 

