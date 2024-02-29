# Criação de contrato (assinatura)

## Exemplo

```json
{
"event": "contract_created",
"createdAt": "2024-01-09T14:45:00.000Z",
	"metadata": {
		"name": "Teste QA Eduzz",
		"email": "testeeduzzqa@eduzz.com",
		"contractId": "3456",
		"productId": [
			"1234"
		]
	},
	"data": {
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
			"isPSL": false,
			"recurrence": {
				"startsAt": "2024-01-15T15:00:00.000Z",
				"nextDue": "2024-02-15T15:00:00.000Z",
				"previousDue": "2024-01-15T15:00:00.000Z",
				"lastDue": "2025-01-09T15:00:00.000Z",
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
}
```

## Dados enviados

| Campo                 | Tipo   | Descrição                           |
|-----------------------|--------|-------------------------------------|