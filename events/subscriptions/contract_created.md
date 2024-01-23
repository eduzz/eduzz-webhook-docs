# Contrato foi criado

## Exemplo

```json
{
  "id": "d4neemljy87rv3og472ag6hl",
  "event": "subscriptions.contract_created",
  "sentDate": "2023-08-31T18:34:23.023Z",
  "data": {
    "producer": {
      "id": "1234",
      "name": "Next Assinaturas",
      "email": "qa-next@eduzz.com"
    },
    "affiliate": {
      "id": "1245",
      "name": "Next Assinaturas Afiliado",
      "email": "qa-next-afiliado@eduzz.com"
    },
    "products": [
      {
        "id": "1234",
        "name": "Produto de assinatura",
        "deliveries": ["file", "external", "nutror", "alpaclass"],
        "price": {
          "currency": "BRL",
          "value": 10.0
        },
        "membershipFee": {
          "currency": "BRL",
          "value": 10.0
        },
        "trial": {
          "isOnTrialPeriod": false,
          "begin": null,
          "finish": null
        }
      }
    ],
    "contract": {
      "id": "3456",
      "paymentMethod": "creditCard",
      "status": "upToDate",
      "createdAt": "2024-01-15T15:00:00.000Z",
      "isPSL": false,
      "totalValue": {
        "currency": "BRL",
        "value": 120.0
      },
      "recurrence": {
        "nextDue": "2024-02-15T15:00:00.000Z",
        "lastDue": "2025-01-09T15:00:00.ver000Z",
        "interval": {
          "type": "month",
          "value": 1
        },
        "totalOfInstallments": 12,
        "isFinite": true,
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
| event                                        | string  | Nome do evento (contract_created)       |
| sentDate                                     | string  | Data do envio                           |
| data.producer.id                             | string  | Id do produtor                          |
| data.producer.name                           | string  | Nome do produtor                        |
| data.producer.email                          | string  | Email do produtor                       |
| data.affiliate.id                            | string  | Id do afiliado                          |
| data.affiliate.email                         | string  | Email do afiliado                       |
| data.affiliate.name                          | string  | Nome do afiliado                        |
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
| data.contract.totalValue.currency            | string  | Tipo de moeda do contrato               |
| data.contract.totalValue.value               | number  | Valor total do contrato                 |
| data.contract.recurrence.nextDue             | string  | Vencimento da próxima fatura            |
| data.contract.recurrence.lastDue             | string  | Vencimento da última fatura             |
| data.contract.recurrence.interval.type       | string  | Tipo de intervalo entre as faturas      |
| data.contract.recurrence.interval.value      | number  | Tempo de intervalo entre as faturas     |
| data.contract.recurrence.totalOfInstallments | number  | Total de parcelas                       |
| data.contract.recurrence.isFinite            | boolean | Contrato é finito                       |
| data.contract.recurrence.price.currency      | string  | Tipo de moeda da parcela                |
| data.contract.recurrence.price.value         | number  | Valor da parcela                        |
| data.customer.name                           | string  | Nome do Aluno                           |
| data.customer.email                          | string  | Email do Aluno                          |
| data.customer.phone                          | string  | Telefone do Aluno                       |
| data.financialResponsible.name               | string  | Nome do responsável financeiro          |
| data.financialResponsible.email              | string  | Email do responsável financeiro         |
| data.financialResponsible.phone              | string  | Telefone do responsável financeiro      |
