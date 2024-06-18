# Aluno finaliza o módulo

## Exemplo 
  
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_finished_module", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
      },
      "module": { 
        "id": "54", 
        "name": "Módulo 1: Aprenda sobre os setores das ações", 
        "finishedAt": "2024-06-12T12:00:10.000Z", 
      },
    } 
} 
``` 

## Dados enviados 

  

| Campo                     | Tipo   | Descrição                                        | 
|---------------------------|--------|--------------------------------------------------| 
| id                        | string | Id do evento                                     | 
| event                     | string | Nome do evento (student_finished_module)         | 
| sentDate                  | string | Data do envio do evento                          |
| data.student.id           | string | Id do aluno na escola                            | 
| data.student.name         | string | Nome do aluno                                    |
| data.module.id            | string | Id do módulo                                     | 
| data.module.name          | string | Nome do módulo                                   | 
| data.module.finishedAt    | string | Data da conclusão do módulo                      | 

