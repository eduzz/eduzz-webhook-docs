# Aluno finaliza o módulo

## Exemplo 
  
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_module_finished", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "457391c9c82bfdcbb4947278c0401e41", 
        "name": "Fulano da Silva",
        "email": "teste@email.com",
      },
      "module": { 
        "id": "22884db148f0ffb0d830ba431102b0b5", 
        "name": "Módulo 1: Aprenda sobre os setores das ações", 
      },
      "course": {
        "id": "046d47672cf6212d201d6e8b0c191e73",
        "name": "elementar"
      },
      "team": {
        "id": "16943848cc6495142a8e3011d0173252",
        "name": "Escola de Teste"
      }
    } 
} 
``` 

## Dados enviados 

  

| Campo                     | Tipo   | Descrição                                        | 
|---------------------------|--------|--------------------------------------------------| 
| id                        | string | Id do evento                                     | 
| event                     | string | Nome do evento (student_module_finished)         | 
| sentDate                  | string | Data do envio do evento                          |
| data.student.id           | string | Id do aluno na escola                            | 
| data.student.name         | string | Nome do aluno                                    |
| data.module.id            | string | Id do módulo                                     | 
| data.module.name          | string | Nome do módulo                                   | 
| data.course.id            | string | Id do curso                                      | 
| data.course.name          | string | Nome do curso                                    | 
| data.team.id              | string | Id da escola                                     | 
| data.team.name            | string | Nome da escola                                   | 

