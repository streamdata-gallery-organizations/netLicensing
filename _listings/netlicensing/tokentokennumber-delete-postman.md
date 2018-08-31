{
  "info": {
    "name": "NetLicensing Delete token",
    "_postman_id": "dcfd262b-fb42-4f8f-94b3-e6f65c82c8f0",
    "description": "Delete a token by number",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "License",
      "item": [
        {
          "id": "fab4a09a-2297-4583-b5df-336a8dfacb19",
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
              "id": "75fb55ac-19c0-4821-bfe5-c6d429c87493"
            }
          ]
        },
        {
          "id": "dca5065f-a702-424f-85ea-54377c5648e5",
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
              "id": "9854fcf5-3902-441f-b833-b6599291d73c"
            }
          ]
        },
        {
          "id": "f7698b66-6c92-481b-b009-e2d9189d6881",
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
              "id": "06a9a195-8cc0-4433-ab47-c652f05e4feb"
            }
          ]
        },
        {
          "id": "81a0cc3d-aa8c-4cc8-8172-70fd4995a2fa",
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
              "id": "39f3b585-e683-4e8e-b680-4d858836e6ce"
            }
          ]
        },
        {
          "id": "08e71571-c733-439a-8ada-d01300cb9f30",
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
              "id": "593419f9-a7d9-460f-a4c0-c02b8ec82602"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensee",
      "item": [
        {
          "id": "f40254a1-b05e-4903-90c2-f91890b7b8e4",
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
              "id": "dcff0a73-51cf-4402-b962-7d163d5d89bb"
            }
          ]
        },
        {
          "id": "833d7a61-8816-4488-8aa9-9a1ae3435ef4",
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
              "id": "0ed44bff-e3ee-4a51-ac5b-b8afbabe7d40"
            }
          ]
        },
        {
          "id": "6874f103-7d75-4930-bb6d-58f7f0706f8f",
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
              "id": "43c58c4b-3cc6-4944-bea6-704e0281e0a3"
            }
          ]
        },
        {
          "id": "936610c0-5cee-481c-b4d0-0afc2ea845a1",
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
              "id": "c53471e7-9bb6-405d-a701-37a1cdd135e9"
            }
          ]
        },
        {
          "id": "6ec3cb6b-0a83-41c4-b8d9-8c0900ddc7bb",
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
              "id": "45de1367-ba2d-4351-9b22-b01521c015cc"
            }
          ]
        },
        {
          "id": "94aa34c5-1e29-4876-832e-10f3c195c7d4",
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
              "id": "9bc734dd-9c4a-4111-8dca-b7dc337b8d1a"
            }
          ]
        },
        {
          "id": "ca2d8ab2-4324-433b-9835-35aa80ed25be",
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
              "id": "da1cf17e-7517-4c3b-9afa-b887a2454f77"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensetemplate",
      "item": [
        {
          "id": "eed4844d-165b-40d9-bbdc-8be76c16c4f3",
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
              "id": "5feb5680-d02f-409d-9eea-5d2a68b7d875"
            }
          ]
        },
        {
          "id": "fc73a005-bdca-47ec-ae28-866720d550f2",
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
              "id": "993156d9-13c3-444e-9fab-18452c92c1ff"
            }
          ]
        },
        {
          "id": "9db90eb4-d7c6-40bf-b14a-64f310c90324",
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
              "id": "9e4ecc86-5486-4ae8-90a4-27eea05aee10"
            }
          ]
        },
        {
          "id": "667ece4b-18c2-4758-93d1-649c61c24daf",
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
              "id": "d2c956d8-9407-4355-90ea-0097289c4f58"
            }
          ]
        },
        {
          "id": "f598de7d-2ffb-483f-ab7e-7259e668b979",
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
              "id": "37875027-9185-4bf3-8db4-7736db77484e"
            }
          ]
        }
      ]
    },
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "ef022350-465c-4ca8-830c-a8b1096cddf7",
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
              "id": "5906732a-e409-47ef-a19c-02b48d1ee9c6"
            }
          ]
        },
        {
          "id": "191c032d-2821-456c-b587-de8dc6fd636f",
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
              "id": "aec35650-5f5f-4fa0-837b-8349f0783e49"
            }
          ]
        },
        {
          "id": "8c1aea80-beb3-4912-ad60-9c500f1a701b",
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
              "id": "3de4e975-851d-4013-b677-476205e752ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "fdcd4f34-fc0e-406a-8dae-78b0e6f4cb74",
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
              "id": "ed231578-b40d-4c95-a6de-68e6676e3aaf"
            }
          ]
        },
        {
          "id": "875de774-c884-4dbe-838a-9ae509595084",
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
              "id": "c89b5590-4995-4976-b447-a7aee37591c2"
            }
          ]
        },
        {
          "id": "a42a508e-9e2c-49bf-81d6-5043c3651e16",
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
              "id": "2a2c776a-5df1-4564-8a6f-c76ce9c8eb1b"
            }
          ]
        },
        {
          "id": "30336e7c-c237-4780-bcfe-a286844bff43",
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
              "id": "ab0704a6-3a7f-48f8-b9ef-d871af67170f"
            }
          ]
        },
        {
          "id": "60a7fc73-c4c2-4445-bf01-ee6aa1176ae9",
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
              "id": "3d6257e0-f03b-468c-b144-b7c22b4f66b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Productmodule",
      "item": [
        {
          "id": "2d8f3e8a-096e-44d3-aff0-558404cf023a",
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
              "id": "2f5c2743-a8ce-4056-b926-5b94cb6725f1"
            }
          ]
        },
        {
          "id": "0211e3a8-0a4c-4b3b-9bd4-6770bc3791ce",
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
              "id": "841c413e-6b1d-4887-af35-6079137c7d0f"
            }
          ]
        },
        {
          "id": "6e05b5a8-78bd-43bd-a38b-ebf349a7f839",
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
              "id": "153ed886-e4ec-433d-87e0-e5c2b11d433f"
            }
          ]
        },
        {
          "id": "f01506fc-4009-4aee-ae09-e57910fc86d2",
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
              "id": "0ca2f631-e75d-4d81-bf20-5627100eaedf"
            }
          ]
        },
        {
          "id": "393b016e-ebed-4cf9-bf1b-35bac0dd3909",
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
              "id": "297ebe5e-a598-4545-ba32-1a4be9d2809a"
            }
          ]
        }
      ]
    },
    {
      "name": "Token",
      "item": [
        {
          "id": "a9f2101d-2b4c-4d30-8d14-d3443e0ccd1b",
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
              "id": "b04b11fd-84cf-4584-bbf6-8bc007a24ae4"
            }
          ]
        },
        {
          "id": "533b0355-30cd-4574-8417-fd6744b83a41",
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
              "id": "fd84e5df-47b1-440e-9c61-c41dd0e6a11c"
            }
          ]
        },
        {
          "id": "06436143-54a5-45c0-ae25-78882286f115",
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
              "id": "b4ab59a1-22e3-4cf4-abfd-8f15f2d6e06a"
            }
          ]
        }
      ]
    }
  ]
}