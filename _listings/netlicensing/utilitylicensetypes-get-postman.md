{
  "info": {
    "name": "NetLicensing License Types list",
    "_postman_id": "3140009d-9bf1-4ffe-aca6-730135d8271d",
    "description": "Return a list of all license types supported by the service",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Utility",
      "item": [
        {
          "id": "664a88b6-1a47-42e3-a8f4-40e531075721",
          "name": "licenseTypes",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/utility/licenseTypes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all license types supported by the service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54f20a58-c836-4bbf-9acc-fc3ef8c77f74"
            }
          ]
        }
      ]
    }
  ]
}