# Condições do contrato foram atualizadas

## Exemplo

```json
{
  "id": "d4neemljy87rv3og472ag6hl",
  "event": "subscriptions.contract_changed",
  "sentDate": "2023-08-31T18:34:23.023Z",
  "data": {
    "changeType": "negotiation",
    "producer": {
      "id": "1234",
      "name": "Next Assinaturas",
      "email": "qa-next@eduzz.com"
    },
    "products": [
      {
        "id": "1234",
        "name": "Produto de assinatura",
        "deliveries": ["nutror"],
        "membershipFee": {
          "currency": "BRL",
          "value": 10.0
        },
        "price": {
          "currency": "BRL",
          "value": 10.0
        },
        "trial": {
          "isOnTrialPeriod": true,
          "begin": "2024-01-15T15:00:00.000Z",
          "finish": "2024-01-30T15:00:00.000Z"
        }
      }
    ],
    "contract": {
      "id": "3456",
      "paymentMethod": "creditCard",
      "status": "upToDate",
      "isPSL": false,
      "createdAt": "2023-01-15T15:00:00.000Z",
      "totalValue": {
        "currency": "BRL",
        "value": null
      },
      "recurrence": {
        "interval": {
          "type": "year",
          "value": 1
        },
        "nextDue": "2025-02-15T15:00:00.000Z",
        "lastDue": null,
        "totalOfInstallments": null,
        "currentInstallment": 2,
        "isFinite": false,
        "price": {
          "currency": "BRL",
          "value": 10.0
        }
      }
    },
    "customer": {
      "name": "Teste QA Eduzz",
      "email": "testeeduzzqa@eduzz.com",
      "phone": "+5515999999999"
    },
    "financialResponsible": {
      "name": "Responsável Financeiro",
      "email": "financial-responsible@eduzz.com",
      "phone": "+5515999999999"
    }
  }
}
```

## Dados enviados

| Campo                                        | Tipo    | Descrição                               |
| -------------------------------------------- | ------- | --------------------------------------- |
| id                                           | string  | Id do evento                            |
| event                                        | string  | Nome do evento (contract_changed)       |
| sentDate                                     | string  | Data do envio                           |
| data.changeType                              | string  | Tipo de atualização do contrato         |
| data.producer.id                             | string  | Id do produtor                          |
| data.producer.name                           | string  | Nome do produtor                        |
| data.producer.email                          | string  | Email do produtor                       |
| data.products[0].id                          | string  | Id do produto                           |
| data.products[0].name                        | string  | Nome do produto                         |
| data.products[0].deliveries[0]               | string  | Tipo de entrega do produto              |
| data.products[0].price.currency              | string  | Tipo de moeda que foi vendido o produto |
| data.products[0].price.value                 | number  | Preço do produto                        |
| data.products[0].membershipFee.currency      | string  | Tipo de moeda da taxa de adesão         |
| data.products[0].membershipFee.value         | number  | Preço da taxa de adesão                 |
| data.products[0].trial.isOnTrialPeriod       | boolean | Contrato está dentro do período trial   |
| data.products[0].trial.begin                 | string  | Data de início do período trial         |
| data.products[0].trial.finish                | string  | Data final do período trial             |
| data.contract.id                             | string  | Id do contrato                          |
| data.contract.paymentMethod                  | string  | Tipo de pagamento do contrato           |
| data.contract.status                         | string  | Status do contrato                      |
| data.contract.isPSL                          | boolean | Contrato é PSL                          |
| data.contract.createdAt                      | string  | Data de criação do contrato             |
| data.contract.totalValue.currency            | string  | Tipo de moeda do contrato               |
| data.contract.totalValue.value               | number  | Valor total do contrato                 |
| data.contract.recurrence.nextDue             | string  | Vencimento da próxima fatura            |
| data.contract.recurrence.previousDue         | string  | Vencimento da fatura anterior           |
| data.contract.recurrence.lastDue             | string  | Vencimento da última fatura             |
| data.contract.recurrence.isFinite            | boolean | Contrato é finito                       |
| data.contract.recurrence.totalOfInstallments | number  | Total de parcelas                       |
| data.contract.recurrence.currentInstallment  | string  | Número da parcela atual do contrato     |
| data.contract.recurrence.interval.type       | string  | Tipo de intervalo entre as faturas      |
| data.contract.recurrence.interval.value      | number  | Tempo de intervalo entre as faturas     |
| data.contract.recurrence.price.currency      | string  | Tipo de moeda da parcela                |
| data.contract.recurrence.price.value         | number  | Valor da parcela                        |
| data.customer.name                           | string  | Nome do Aluno                           |
| data.customer.email                          | string  | Email do Aluno                          |
| data.customer.phone                          | string  | Telefone do Aluno                       |
| data.financialResponsible.name               | string  | Nome do responsável financeiro          |
| data.financialResponsible.email              | string  | Email do responsável financeiro         |
| data.financialResponsible.phone              | string  | Telefone do responsável financeiro      |
