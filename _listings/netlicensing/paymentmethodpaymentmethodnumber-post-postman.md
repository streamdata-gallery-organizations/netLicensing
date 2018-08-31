{
  "info": {
    "name": "NetLicensing Update payment method",
    "_postman_id": "deefec99-9378-4e8f-b983-05076e9a64ae",
    "description": "Sets the provided properties to a payment method. Return an updated payment method",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "6ad0c432-359c-4d91-b1f9-5c904fd15c62",
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
              "id": "c52b2e7d-01be-4349-ba52-c981e39c651b"
            }
          ]
        },
        {
          "id": "a9b2b671-b56f-41c9-9284-2853f1b69898",
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
              "id": "7dceb841-26d6-41bc-a19a-1c6593a3a740"
            }
          ]
        },
        {
          "id": "cd0f9ef5-d566-4a61-a07b-cedb6b1ced47",
          "name": "updatePaymentMethod",
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
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to false, the payment method is disabled"
                },
                {
                  "key": "paypal.subject",
                  "value": "{}",
                  "disabled": false,
                  "description": "The e-mail address of the PayPal account for which you are making the API calls"
                }
              ]
            },
            "description": "Sets the provided properties to a payment method. Return an updated payment method"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7afaa79-eccf-47f9-992e-9d709d9f6f61"
            }
          ]
        }
      ]
    }
  ]
}