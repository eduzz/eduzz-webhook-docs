# Aluno acessa o certificado

## Exemplo 
  
```json 
{ 
    "id": "4c832x3ynl8dwe7454941xzr5", 
    "event": "alpaclass.student_certificate_accessed", 
    "sentDate": "2024-06-12T12:00:10.000Z", 
    "data": { 
      "student": { 
        "id": "1", 
        "name": "Fulano da Silva",
        "email": "fulano.silva@email.com"
      },
      "course": { 
        "id": "54", 
        "name": "Day trade para iniciantes", 
      },
      "team": { 
        "id": "54", 
        "name": "Escola de Hudson", 
      },
      "certificateUrl": "https://certificados.alpaclass.testzz.ninja/download/ZJ1zjj/certificado.pdf", 
    } 
} 
``` 

## Dados enviados 

| Campo                   | Tipo   | Descrição                                        | 
|-------------------------|--------|--------------------------------------------------| 
| id                      | string | Id do evento                                     | 
| event                   | string | Nome do evento (student_certificate_accessed)    | 
| sentDate                | string | Data do envio do evento                          |
| data.student.id         | string | Id do aluno na escola                            | 
| data.student.name       | string | Nome do aluno                                    |
| data.student.email      | string | E-mail do aluno                                  |
| data.course.id          | string | Id do curso                                      | 
| data.course.name        | string | Nome do curso                                    | 
| data.team.id            | string | Id da escola                                     | 
| data.team.name          | string | Nome da escola                                   | 
| data.certificateUrl     | string | Url do certificado                               | 
