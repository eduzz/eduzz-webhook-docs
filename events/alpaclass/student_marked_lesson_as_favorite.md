# Aluno marca aula como favorita

## Exemplo 
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_marked_lesson_as_favorite", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva", 
      },
      "lesson": { 
        "id": "54", 
        "name": "Aula 1 - Melhores ações do setor de energia", 
        "actionDate": "2024-06-12T12:00:10.000Z", 
      },
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                        | 
|---------------------------|--------|--------------------------------------------------| 
| id                        | string | Id do evento                                     | 
| event                     | string | Nome do evento (student_marked_lesson_as_favorite) | 
| sentDate                  | string | Data do envio do evento                          |
| data.student.id           | string | Id do aluno na escola                            | 
| data.student.name         | string | Nome do aluno                                    |
| data.lesson.id            | string | Id da aula                                       | 
| data.lesson.name          | string | Nome da aula                                     | 
| data.lesson.actionDate    | string | Data da ação                                     | 

