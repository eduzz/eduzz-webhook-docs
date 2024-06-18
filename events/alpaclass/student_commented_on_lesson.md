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
        "name": "Agiotagem para iniciantes passo 1", 
      },
      "comment": {
        "body": "Adorei a aula, espero conseguir aplicar os aprendizados!",
        "createdAt": "2024-06-12T12:00:10.000Z", 
      }
    } 
} 
``` 

## Dados enviados 

| Campo                     | Tipo   | Descrição                                   | 
|---------------------------|--------|---------------------------------------------| 
| id                        | string | Id do evento                                | 
| event                     | string | Nome do evento (student_commented_on_lesson)| 
| sentDate                  | string | Data do envio do evento                     |
| data.student.id           | number | Id do aluno na escola                       | 
| data.student.name         | string | Nome do aluno                               |
| data.lesson.id            | number | Id da aula                                  | 
| data.lesson.name          | string | Nome da aula                                | 
| data.comment.body         | string | Conteúdo do comentário                      | 
| data.comment.createdAt    | string | Data da criação do comentário               | 

