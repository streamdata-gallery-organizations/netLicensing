{
  "info": {
    "name": "NetLicensing Get payment method",
    "_postman_id": "1b742b51-f176-425e-b7c4-61f8dd90ddc7",
    "description": "Return a payment method info by paymentMethodNumber",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "d71a2ef1-768a-4b3f-b7bf-f381c31e526d",
          "name": "listPaymentMethods",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/paymentmethod",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all payment methods for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b2637a0-2d74-498b-8de1-9fb71b203481"
            }
          ]
        },
        {
          "id": "7af70b96-a6f2-43cb-a605-a74615ed9533",
          "name": "getPaymentMethod",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "paymentmethod/:paymentMethodNumber"
              ],
              "variable": [
                {
                  "id": "paymentMethodNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a payment method info by paymentMethodNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f331f89b-e82a-49c0-9fbc-db5e9b35d701"
            }
          ]
        }
      ]
    }
  ]
}