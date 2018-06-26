{
  "info": {
    "name": "NetLicensing Payment Methods list",
    "_postman_id": "23a6553c-faa0-4870-8ce4-1733472efeee",
    "description": "Return a list of all payment methods for the current vendor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "da9e932c-fcea-43e1-a912-1ab63bf7c90f",
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
              "id": "b4b80590-6cb4-459c-bb13-73fd65a00d99"
            }
          ]
        }
      ]
    }
  ]
}