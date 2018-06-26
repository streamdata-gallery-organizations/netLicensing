{
  "info": {
    "name": "NetLicensing Get transaction",
    "_postman_id": "869b3c23-97ab-4320-b20c-838352e7e0b7",
    "description": "Return a transaction by transactionNumber",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "License",
      "item": [
        {
          "id": "98075026-ed87-46ad-aa2c-8e203d801e9b",
          "name": "listLicenses",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/license",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all licenses for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92d75a2a-7dd1-42ff-ab5e-dba7ce6a6c5c"
            }
          ]
        },
        {
          "id": "2b77ab3b-59a8-4f5e-92d6-a288327dac36",
          "name": "createLicense",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/license",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": "Specifies currency for the license price"
                },
                {
                  "key": "hidden",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, this license is not shown in NetLicensing Shop as purchased license"
                },
                {
                  "key": "licenseeNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "licenseTemplateNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name for the licensed item"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "parentfeature",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for TIMEVOLUME license type and RENTAL licensing model"
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": "Price for the license"
                },
                {
                  "key": "startDate",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for TIMEVOLUME license type"
                },
                {
                  "key": "timeVolume",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for TIMEVOLUME license type"
                }
              ]
            },
            "description": "Creates a new license"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2104fad1-9abc-40c3-87bd-fe53d5f3dd49"
            }
          ]
        },
        {
          "id": "fad32fd1-9484-432a-b151-35799d18f34e",
          "name": "getLicense",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "license/:licenseNumber"
              ],
              "variable": [
                {
                  "id": "licenseNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get license by a licenseNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "528ee494-cb2a-4445-b15b-116647ac1979"
            }
          ]
        },
        {
          "id": "42e65b99-2eb0-438f-94bb-c88a52cc8669",
          "name": "updateLicense",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "license/:licenseNumber"
              ],
              "variable": [
                {
                  "id": "licenseNumber",
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
                  "description": ""
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": "Specifies currency for the license price"
                },
                {
                  "key": "hidden",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, this license is not shown in NetLicensing Shop as purchased license"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name for the licensed item"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number (across all products/licensees of a vendor) that identifies the license"
                },
                {
                  "key": "parentfeature",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": "Price for the license"
                },
                {
                  "key": "startDate",
                  "value": "{}",
                  "disabled": false,
                  "description": "for TIMEVOLUME licenseType"
                },
                {
                  "key": "timeVolume",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Update license by a licenseNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f1b56d8-5ef2-4392-ba4a-d2999e0dc0c7"
            }
          ]
        },
        {
          "id": "dea40d9d-0a2a-4488-9c31-8772728e3880",
          "name": "deleteLicense",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "license/:licenseNumber"
              ],
              "variable": [
                {
                  "id": "licenseNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete license by a licenseNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b67ea0fb-3ab0-4f15-973c-f8446a3a3823"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensee",
      "item": [
        {
          "id": "5c12ddeb-1d3d-440e-8eee-b400cec69233",
          "name": "listLicensees",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/licensee",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all licensees for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c4d888f-eb8f-4197-a4d8-9ed583da8dc6"
            }
          ]
        },
        {
          "id": "e44286e2-ec30-4c70-9e0f-0bf665038314",
          "name": "createLicensee",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/licensee",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to false, the licensee is disabled"
                },
                {
                  "key": "licenseeSecret",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee Secret for licensee"
                },
                {
                  "key": "markedForTransfer",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mark licensee for transfer"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number (across all products of a vendor) that identifies the licensee"
                },
                {
                  "key": "productNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "productNumber to assign new licensee object"
                }
              ]
            },
            "description": "Creates a new licensee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64317e51-0bfc-4b01-8f37-61407c6368c5"
            }
          ]
        },
        {
          "id": "78dbf6dd-a90c-4e36-af5a-a3237a193b83",
          "name": "getLicensee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensee/:licenseeNumber"
              ],
              "variable": [
                {
                  "id": "licenseeNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a licensee by licenseeNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84653ff0-2a52-4c2f-bfa5-53698f3d2620"
            }
          ]
        },
        {
          "id": "18271dd9-d9e6-42f7-bb61-edd440584033",
          "name": "updateLicensee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensee/:licenseeNumber"
              ],
              "variable": [
                {
                  "id": "licenseeNumber",
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
                  "description": "If set to false, the licensee is disabled"
                },
                {
                  "key": "licenseeSecret",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee Secret for licensee"
                },
                {
                  "key": "markedForTransfer",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mark licensee for transfer"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "New licensee number (update)"
                }
              ]
            },
            "description": "Sets the provided properties to a licensee. Return an updated licensee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e55bf7e0-f8af-4304-b3ee-0b70edfb094c"
            }
          ]
        },
        {
          "id": "24fb9112-fac0-4f62-8251-10c35fa301a1",
          "name": "deleteLicensee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensee/:licenseeNumber"
              ],
              "query": [
                {
                  "key": "forceCascade",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "licenseeNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a licensee by number"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cefb64a6-242f-422b-8d59-488706444ac8"
            }
          ]
        },
        {
          "id": "4c6a2a96-b703-47a4-87c8-27d5456677a6",
          "name": "transferLicenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensee/:licenseeNumber/transfer"
              ],
              "variable": [
                {
                  "id": "licenseeNumber",
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
                  "key": "sourceLicenseeNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee number which licenses to be transferred"
                }
              ]
            },
            "description": "Licenses transfer between licensees"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53476296-05f5-41cf-ad49-63debe8364fb"
            }
          ]
        },
        {
          "id": "967eb1da-520c-4be4-81ff-49068dd1da23",
          "name": "validateLicensee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensee/:licenseeNumber/validate"
              ],
              "variable": [
                {
                  "id": "licenseeNumber",
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
                  "key": "licenseeName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Human-readable name for the auto-created licensee (will be set as custom Licensee property)"
                },
                {
                  "key": "licenseeSecret",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee Secret key for licensee"
                },
                {
                  "key": "productNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product number, must be provided when licensee auto-create is enabled (see also Product JavaDoc)"
                }
              ]
            },
            "description": "Validates active licenses of the licensee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb446611-64bf-4db2-8e57-2d3d89b3d72a"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensetemplate",
      "item": [
        {
          "id": "2afbb42d-86df-4186-bb13-a98598fb4866",
          "name": "listLicenseTemplates",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/licensetemplate",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all license templates for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc80d982-2bec-4761-b90b-3e27c80cc56b"
            }
          ]
        },
        {
          "id": "1b4d6fbf-f75b-4c7f-b108-ce64b4ac2046",
          "name": "createLicenseTemplate",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/licensetemplate",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to false, the license template is disabled"
                },
                {
                  "key": "automatic",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, every new licensee automatically gets one license out of this license template on creation"
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": "specifies currency for the license price"
                },
                {
                  "key": "hidden",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, this license template is not shown in NetLicensing Shop as offered for purchase"
                },
                {
                  "key": "hideLicenses",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, licenses from this license template are not visible to the end customer, but participate in validation"
                },
                {
                  "key": "licenseType",
                  "value": "{}",
                  "disabled": false,
                  "description": "type of licenses created from this license template"
                },
                {
                  "key": "maxSessions",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for FLOATING license type"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "license template name to reate license template object"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "lUnique number (across all products of a vendor) that identifies the license template"
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": "price for the license"
                },
                {
                  "key": "productModuleNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "Number of product module to reate license template object"
                },
                {
                  "key": "timeVolume",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for TIMEVOLUME license type"
                }
              ]
            },
            "description": "Creates a new license template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "097de580-16a5-42b6-b6d2-4cd875eaa220"
            }
          ]
        },
        {
          "id": "2ef7f860-8b55-4152-a631-ca6a247baaa7",
          "name": "getLicenseTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensetemplate/:licenseTemplateNumber"
              ],
              "variable": [
                {
                  "id": "licenseTemplateNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a license template by licenseTemplateNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80ca2ba6-d6fc-4671-8283-d5eb58679cdf"
            }
          ]
        },
        {
          "id": "8f93ccbf-d107-46e5-9708-12605d6e8112",
          "name": "updateLicenseTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensetemplate/:licenseTemplateNumber"
              ],
              "variable": [
                {
                  "id": "licenseTemplateNumber",
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
                  "description": "If set to false, the license template is disabled"
                },
                {
                  "key": "automatic",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, every new licensee automatically gets one license out of this license template on creation"
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": "Specifies currency for the license price"
                },
                {
                  "key": "hidden",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, this license template is not shown in NetLicensing Shop as offered for purchase"
                },
                {
                  "key": "hideLicenses",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, licenses from this license template are not visible to the end customer, but participate in validation"
                },
                {
                  "key": "licenseType",
                  "value": "{}",
                  "disabled": false,
                  "description": "type of licenses created from this license template"
                },
                {
                  "key": "maxSessions",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for FLOATING license type"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name for the licensed item"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "New license template number (update)"
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": "Price for the license"
                },
                {
                  "key": "timeVolume",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mandatory for TIMEVOLUME license type"
                }
              ]
            },
            "description": "Sets the provided properties to a license template. Return an updated license template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20b83f61-0bd4-4f17-be63-64dcb7f1fd15"
            }
          ]
        },
        {
          "id": "de3c5d0f-d2af-42b2-b8cb-650c6abd28d8",
          "name": "deleteLicenseTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "licensetemplate/:licenseTemplateNumber"
              ],
              "query": [
                {
                  "key": "forceCascade",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "licenseTemplateNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a license template by number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "894ad319-8cf2-4b10-911a-8c5cc6a90fb2"
            }
          ]
        }
      ]
    },
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "e998f4a4-ebec-4535-aa42-fcf00aae93af",
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
              "id": "44585bcd-aeb9-45c2-8d35-d3184e7c1c7c"
            }
          ]
        },
        {
          "id": "cd90bb43-2dc6-4f4d-9256-647d014ef0a1",
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
              "id": "e63ca3de-8a7f-46a5-94c1-eb52e752f72e"
            }
          ]
        },
        {
          "id": "659c5e6d-7926-4e34-bbf8-c2062c85c947",
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
              "id": "bfa8880a-fb6f-45ba-b63e-84adf5b8783a"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "435e2e29-9dde-49f3-8b3b-dd503b0774b9",
          "name": "listProducts",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/product",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all configured products for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f89c290-08c0-4d7f-a4a4-73cbe01aacb4"
            }
          ]
        },
        {
          "id": "6d5b5470-2a74-48a9-968e-731c5f6f7db4",
          "name": "createProduct",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/product",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to false, the product is disabled"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product description"
                },
                {
                  "key": "licenseeAutoCreate",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, non-existing licensees will be created at first validation attempt"
                },
                {
                  "key": "licenseeSecretMode",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee secret mode for product"
                },
                {
                  "key": "licensingInfo",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensing information"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product name"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number that identifies the product"
                },
                {
                  "key": "vatMode",
                  "value": "{}",
                  "disabled": false,
                  "description": "Vat mode for product"
                },
                {
                  "key": "version",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product version"
                }
              ]
            },
            "description": "Creates a new product"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff48bf06-f060-4081-931a-ba60aae0d467"
            }
          ]
        },
        {
          "id": "82fe82d5-aad7-45af-ab40-554b634229aa",
          "name": "productNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "product/:productNumber"
              ],
              "variable": [
                {
                  "id": "productNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a product by productNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afdce292-45ae-4617-90ab-7ae1c0595725"
            }
          ]
        },
        {
          "id": "84d8e36d-8020-4b9c-a828-85a8aed59120",
          "name": "updateProduct",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "product/:productNumber"
              ],
              "variable": [
                {
                  "id": "productNumber",
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
                  "description": "If set to false, the product is disabled"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product description"
                },
                {
                  "key": "licenseeAutoCreate",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to true, non-existing licensees will be created at first validation attempt"
                },
                {
                  "key": "licenseeSecretMode",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensee secret mode for product"
                },
                {
                  "key": "licensingInfo",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensing information"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product name"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "New product number (update)"
                },
                {
                  "key": "vatMode",
                  "value": "{}",
                  "disabled": false,
                  "description": "Vat mode for product"
                },
                {
                  "key": "version",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product version"
                }
              ]
            },
            "description": "Sets the provided properties to a product. Return an updated product"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9a5904-0755-4868-8a30-567f66f962f5"
            }
          ]
        },
        {
          "id": "a5f3bedc-61b3-4f96-b059-55a05a9a3290",
          "name": "deleteProduct",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "product/:productNumber"
              ],
              "query": [
                {
                  "key": "forceCascade",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "productNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a product by number"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b48e7d6d-6125-41cf-bbde-2e9147169c33"
            }
          ]
        }
      ]
    },
    {
      "name": "Productmodule",
      "item": [
        {
          "id": "bb46363f-8ac7-431a-92b8-8d3a33fef7a7",
          "name": "listProductModules",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/productmodule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all product modules for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da8f8b5f-8a21-4271-b6ab-ddc6f82141ff"
            }
          ]
        },
        {
          "id": "c87f47f6-7363-4a83-a1a2-2d1eb230fea5",
          "name": "createProductModule",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/productmodule",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "If set to false, the product module is disabled"
                },
                {
                  "key": "licenseTemplate",
                  "value": "{}",
                  "disabled": false,
                  "description": "License template"
                },
                {
                  "key": "licensingModel",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensing model applied to this product module"
                },
                {
                  "key": "maxCheckoutValidity",
                  "value": "{}",
                  "disabled": false,
                  "description": "Maximum checkout validity (days)"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product module name that is visible to the end customers in NetLicensing Shop"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number (across all products of a vendor) that identifies the product module"
                },
                {
                  "key": "productNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number (across all products of a vendor) that identifies the product module"
                },
                {
                  "key": "redThreshold",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remaining time volume for red level"
                },
                {
                  "key": "yellowThreshold",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remaining time volume for yellow level"
                }
              ]
            },
            "description": "Creates a new product module"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b0a2260-99be-4a97-b92f-8602aa447b21"
            }
          ]
        },
        {
          "id": "e4e0558f-a0d6-48e4-82ff-9e0dd6f5ca8f",
          "name": "getProductModule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "productmodule/:productModuleNumber"
              ],
              "variable": [
                {
                  "id": "productModuleNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a product module by productModuleNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d9e6eab-7ec5-4840-a2f6-013f9511fea9"
            }
          ]
        },
        {
          "id": "5bf1fed1-647e-48be-9388-f800ad73593e",
          "name": "updateProductModule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "productmodule/:productModuleNumber"
              ],
              "variable": [
                {
                  "id": "productModuleNumber",
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
                  "description": "If set to false, the product module is disabled"
                },
                {
                  "key": "licenseTemplate",
                  "value": "{}",
                  "disabled": false,
                  "description": "License template"
                },
                {
                  "key": "licensingModel",
                  "value": "{}",
                  "disabled": false,
                  "description": "Licensing model applied to this product module"
                },
                {
                  "key": "maxCheckoutValidity",
                  "value": "{}",
                  "disabled": false,
                  "description": "Maximum checkout validity (days)"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Product module name that is visible to the end customers in NetLicensing Shop"
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "New product module number (update)"
                },
                {
                  "key": "redThreshold",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remaining time volume for red level"
                },
                {
                  "key": "yellowThreshold",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remaining time volume for yellow level"
                }
              ]
            },
            "description": "Sets the provided properties to a product module. Return an updated product module"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65d04b00-b423-41a5-a005-ef80a94ce4a1"
            }
          ]
        },
        {
          "id": "06664e5f-34be-470e-b155-b70cd9c54a78",
          "name": "deleteProductModule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "productmodule/:productModuleNumber"
              ],
              "query": [
                {
                  "key": "forceCascade",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "productModuleNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a product module by number"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "790c2345-f419-47d2-8d40-a55ab5de2f5b"
            }
          ]
        }
      ]
    },
    {
      "name": "Token",
      "item": [
        {
          "id": "927433f8-2d9b-465a-9eb2-a52e6868dfc1",
          "name": "listTokens",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all tokens for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f455c102-a2ca-4031-80f0-155748b1dbf1"
            }
          ]
        },
        {
          "id": "4fa09d8c-b6c8-4e6d-8bb5-8abff2270068",
          "name": "createToken",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/token",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "cancelURL",
                  "value": "{}",
                  "disabled": false,
                  "description": "for tokenType=SHOP only; take customers to this URL when they cancel their checkout"
                },
                {
                  "key": "cancelURLTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": "for tokenType=SHOP only; shop link title for cancel checkout process"
                },
                {
                  "key": "licenseeNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "for tokenType=SHOP only (mandatory); identifies licensee that will be assigned to the shop token"
                },
                {
                  "key": "successURL",
                  "value": "{}",
                  "disabled": false,
                  "description": "for tokenType=SHOP only; take customers to this URL when they finish checkout"
                },
                {
                  "key": "successURLTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": "for tokenType=SHOP only; shop link title for successful checkout process"
                },
                {
                  "key": "tokenType",
                  "value": "{}",
                  "disabled": false,
                  "description": "Token type to be generated"
                }
              ]
            },
            "description": "Create token by tokenType and additional token parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edd266db-96dd-4a6c-9bfe-0d2870541a3d"
            }
          ]
        },
        {
          "id": "ea749bf7-b6f1-456d-bf50-5607d9ab5c11",
          "name": "getToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "token/:tokenNumber"
              ],
              "variable": [
                {
                  "id": "tokenNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a token by tokenNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a87a65a-aa85-4ffe-a24f-427b231e371d"
            }
          ]
        },
        {
          "id": "b906c3bf-bc63-4e12-9c4b-7bfb184342dc",
          "name": "deleteToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "token/:tokenNumber"
              ],
              "variable": [
                {
                  "id": "tokenNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a token by number"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c0cb7aa-bbe5-4fc2-8070-a46987da5496"
            }
          ]
        }
      ]
    },
    {
      "name": "Transaction",
      "item": [
        {
          "id": "78611a0d-7b88-457d-9aad-af6cea383888",
          "name": "listTransactions",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/transaction",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of all transactions for the current vendor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05d296de-114e-4ea4-a925-b636e927c5cc"
            }
          ]
        },
        {
          "id": "f21339d4-2741-40ce-900f-66ca10ad1d90",
          "name": "createTransaction",
          "request": {
            "url": "http://go.netlicensing.io/core/v2/rest/transaction",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "always true for transactions"
                },
                {
                  "key": "dateClosed",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "dateCreated",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "licenseeNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "number",
                  "value": "{}",
                  "disabled": false,
                  "description": "Unique number (across all products of a vendor) that identifies the transaction"
                },
                {
                  "key": "paymentMethod",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "source",
                  "value": "{}",
                  "disabled": false,
                  "description": "AUTO transaction for internal use only"
                },
                {
                  "key": "status",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new transaction"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11edb80e-aa61-457d-9c4a-4fdc79b880e1"
            }
          ]
        },
        {
          "id": "72bf2536-a1d6-4a1d-82b4-c0cb0a95ecea",
          "name": "getTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.netlicensing.io",
              "path": [
                "core",
                "v2",
                "rest",
                "transaction/:transactionNumber"
              ],
              "variable": [
                {
                  "id": "transactionNumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a transaction by transactionNumber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5972562e-2fd4-46a9-af74-d1b86b8b5977"
            }
          ]
        }
      ]
    }
  ]
}