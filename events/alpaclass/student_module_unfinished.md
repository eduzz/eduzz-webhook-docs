# Aluno desmarca como finalizado o módulo

## Exemplo 
  
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_module_unfinished", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva",
        "email": "teste@email.com",
      },
      "module": { 
        "id": "54", 
        "name": "Módulo 1: Aprenda sobre os setores das ações", 
      },
      "course": {
        "id": "162",
        "name": "elementar"
      },
      "team": {
        "id": "538",
        "name": "Escola de Hudson"
      }
    } 
} 
``` 

## Dados enviados 

  

| Campo                     | Tipo   | Descrição                                        | 
|---------------------------|--------|--------------------------------------------------| 
| id                        | string | Id do evento                                     | 
| event                     | string | Nome do evento (student_module_unfinished)       | 
| sentDate                  | string | Data do envio do evento                          |
| data.student.id           | string | Id do aluno na escola                            | 
| data.student.name         | string | Nome do aluno                                    |
| data.module.id            | string | Id do módulo                                     | 
| data.module.name          | string | Nome do módulo                                   | 
| data.course.id            | string | Id do curso                                      | 
| data.course.name          | string | Nome do curso                                    | 
| data.team.id              | string | Id da escola                                     | 
| data.team.name            | string | Nome da escola                                   | 

