# Atualização de contrato (assinatura)

## Exemplo

```json
{
	"producer": {
		"id": "1234",
		"name": "Next Assinaturas",
		"email": "qa-next@eduzz.com"
	},
	"products": [
		{
			"id": "1234",
			"name": "Produto de assinatura",
			"deliveries": [
				"file",
				"external",
				"nutror",
				"alpaclass"
			],
			"plan": null,
			"price": {
				"currency": "BRL",
				"value": 10.0
			},
			"membershipFee": {
				"currency": "BRL",
				"value": 10.0
			}
		}
	],
	"contract": {
		"id": "3456",
		"payment": {
			"method": "creditCard",
			"totalOfInstallments": 12
		},
		"status": "upToDate",
		"trialDays": 0,
		"createdAt": "2024-01-15T15:00:00.000Z",
		"updatedAt": "2024-01-15T15:00:00.000Z",
		"contentAccess": {
			"removeOnContractEnd": true,
			"removeOnLatePayment": true
		},
		"isUnlimitedInstallments": false,
		"recurrence": {
			"startsAt": "2024-01-15T15:00:00.000Z",
			"nextDue": "2024-02-15T15:00:00.000Z",
			"currentDue": "2024-01-15T15:00:00.000Z",
			"finalDue": "2025-01-09T15:00:00.000Z",
			"finishesAt": "2025-01-09T15:00:00.000Z",
			"frequency": {
				"type": "month",
				"value": 1
			},
			"charges": {
				"total": 1,
				"current": 1
			},
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
		"phone": {
			"countryCode": "55",
			"areaCode": "15",
				"number":  "5999999999"
		}
	},
	"financialResponsible": {
		"name": "Responsável Financeiro",
		"email": "financial-responsible@eduzz.com",
		"phone": {
			"countryCode": "55",
			"areaCode": "15",
			"number":  "5999999999"
		}
	}
}
```

## Dados enviados


| Campo                                           | Tipo   |     Descrição                                        |
|-------------------------------------------------|--------|------------------------------------------------------|
| event                                           | string | nome do evento(contract_updated)                     |
| createdAt                                       | string | data de criação do evento                            |
| data.producer.id                                | string | id do produtor                                       |
| data.producer.name                              | string | nome do produtor                                     |
| data.producer.email                             | string | email do produtor                                    |
| data.products.id                                | string | id do produto                                        |
| data.products.name                              | string | nome do produto                                      |
| data.products.delivery                          | string | forma de entrega do produto                          |
| data.products.plan                              | string | plano do produto                                     |
| data.products.price.currency                    | string | moeda usada no produto                               |
| data.products.price.value                       | number | valor do produto                                     |
| data.products.membershipFee.currency            | string | moeda da taxa de adesão do produto                   |
| data.products.membershipFee.value               | number | valor da taxa de adesão do produto                   |
| contract.id                                     | string | id do contrato                                       |
| contract.payment.method                         | string | forma de pagamento                                   |
| contract.payment.totalOfInstallments            | number | numero de parcelas                                   |
| contract.status                                 | string | status do contrato                                   |
| contract.trialDays                              | number | dias de teste                                        |
| contract.createdAt                              | string | data de criação do contrato                          |
| contract.updateAt                               | string | data de atualização do contrato                      |
| contract.contentAccess.removeOnContractEnd      | bool   | remover acesso ao conteúdo no final do contrato      |
| contract.contentAccess.removeOnLatePayment      | bool   | remover acesso ao conteúdo de pagamento com atraso   |
| contract.isPSL                                  | bool   | se o contrato é PSL(parcelamento sem limite)         |
| contract.recurrence.startAt                     | string | data de inicio do contrato                           |
| contract.recurrence.nextDue                     | string | data do próximo vencimento                           |
| contract.recurrence.currentDue                  | string | data atual do contrato                               |
| contract.recurrence.finalDue                    | string | data do último vencimento                            |
| contract.recurrence.finishesAt                  | string | data do termino do contrato                          |
| contract.recurrence.frequency.type              | string | tipo de frequência da cobrança                       |
| contract.recurrence.frequency.value             | number | valor referente a frequência da cobrança             |
| contract.recurrence.charges.total               | number | número de cobranças                                  |
| contract.recurrence.charges.current             | number | moeda usada nas cobranças                            |
| contract.recurrence.isFinite                    | bool   | se é finito ou infinito                              |
| contract.price.currency                         | string | moeda usada no preço                                 |
| contract.price.value                            | number |  valor do contrato                                   |
| customer.name                                   | string | nome do cliente                                      |
| customer.email                                  | string | email do cliente                                     |
| customer.phone.countryCode                      | string | código de telefone do pais do cliente                |
| customer.phone.areaCode                         | string | codigo de área do cliente                            |
| customer.phone.number                           | string | número de telefone do cliente                        |
| customer.financialResponsible.name              | string | nome do resposável financeiro                        |
| customer.financialResponsible.email             | string | email do responsável financeiro                      |
| customer.financialResponsible.phone.countryCode | string | código de telefone do pais do resposável financeiro  |
| customer.financialResponsible.phone.areaCode    | string | codigo de área do responsável financeiro             |
| customer.financialResponsible.phone.number      | string | número de telefone do responsável financeiro         |
