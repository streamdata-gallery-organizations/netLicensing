{
  "info": {
    "name": "NetLicensing Licensing Models list",
    "_postman_id": "5d982e2c-3bb5-4373-aa37-c6536e9a61ed",
    "description": "Return a list of all licensing models supported by the service",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Utility",
      "item": [
        {
          "id": "71dd1b83-8993-49f8-8645-7a346991c9b9",
          "name": "licensingModels",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/utility/licensingModels",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all licensing models supported by the service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f6004bb-cf0a-4918-ad26-09493a9ba6bd"
            }
          ]
        }
      ]
    }
  ]
}