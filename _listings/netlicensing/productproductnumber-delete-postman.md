{
  "info": {
    "name": "NetLicensing Delete product",
    "_postman_id": "ce241193-0960-431c-8447-fb6cd77063f9",
    "description": "Delete a product by number",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "License",
      "item": [
        {
          "id": "5ccbb498-1026-4db2-a8ae-36bd5ade8ced",
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
              "id": "9ed4ee60-e64c-4679-a8c7-1f896e9fe311"
            }
          ]
        },
        {
          "id": "ef34a075-433e-4403-a300-ccf95edfe280",
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
              "id": "dc5f0687-8fce-4237-aba1-e636725886d1"
            }
          ]
        },
        {
          "id": "864d1648-b9f6-4857-9211-2e4d416dd918",
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
              "id": "644ac869-0634-4cb1-9979-c3924909d437"
            }
          ]
        },
        {
          "id": "9fb20cae-3529-4d84-a911-4123b80c22b4",
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
              "id": "831b8293-9b2a-4d75-9d1e-f9ac61f7b830"
            }
          ]
        },
        {
          "id": "ea293dbd-2d33-4b12-a591-87169d2f4283",
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
              "id": "cf0a0cd7-f449-4b86-9ded-535819d39205"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensee",
      "item": [
        {
          "id": "d2719102-d1dd-4c1f-964a-2bc6a8e2f3ec",
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
              "id": "c772848a-ac44-4f55-8919-c514d4f9d297"
            }
          ]
        },
        {
          "id": "01cb0599-6a49-4392-bda3-b753d163c0ff",
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
              "id": "94e58b6c-b07e-4741-ac35-c66c52d34009"
            }
          ]
        },
        {
          "id": "4aa51fb6-fa86-4467-9f0a-7c92254f1edf",
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
              "id": "9ba5955c-2c96-4fb7-b269-47af588fbc84"
            }
          ]
        },
        {
          "id": "cb03da11-9003-4b9e-bc6b-7dd4d9b96fee",
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
              "id": "788a8399-c72c-4cf1-afbb-abf863bb31a1"
            }
          ]
        },
        {
          "id": "71e1b90b-3048-4d31-9894-15ad09cc060c",
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
              "id": "5860f060-6fd2-4b06-860a-4691255f5a73"
            }
          ]
        },
        {
          "id": "b649fe02-782b-4486-9abd-c3d01297f16e",
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
              "id": "ab2a9c9e-dce9-486a-b738-d3ddcd556548"
            }
          ]
        },
        {
          "id": "61ae3eed-033c-4447-9520-64f04f466e6b",
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
              "id": "f9d11e55-4e29-4121-90d2-0394a0d1f366"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensetemplate",
      "item": [
        {
          "id": "a6088970-05a3-43ba-8de9-b33b9d3e6f22",
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
              "id": "760d4307-41fb-4759-bbbd-02e4ba47e869"
            }
          ]
        },
        {
          "id": "4e79e398-80a1-443e-b5d5-d8eebedf6a4e",
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
              "id": "bfba19a3-251d-42d1-bd1f-83c18ccc7912"
            }
          ]
        },
        {
          "id": "cdd91a5f-21b2-4024-bd2c-fa91ecc076d7",
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
              "id": "c5829ff6-c820-4644-8700-6da693d35be3"
            }
          ]
        },
        {
          "id": "f4769e28-ee07-4b2c-82a3-7b9d5ba1e8ee",
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
              "id": "f3616af4-44f0-42c4-82e3-68eae166b8b5"
            }
          ]
        },
        {
          "id": "fa9d7789-7f0d-4b2a-82e8-12a1e35b4b9c",
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
              "id": "0890c93c-0d31-4521-83b4-9fc9ad9df9f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "f93387b4-31c3-4ae0-bd07-262a0fdbe2b4",
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
              "id": "3ee193ff-d053-49ae-9b5e-9f1626188fc7"
            }
          ]
        },
        {
          "id": "3f211305-5af7-403d-9280-31383ea490bf",
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
              "id": "31b61d5b-1a3d-44e9-be54-0947a497b4e5"
            }
          ]
        },
        {
          "id": "08f69817-59af-4f76-8c0d-c99c55516d28",
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
              "id": "bee180d1-aba6-4e2b-ab58-449750b21698"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "2252a3ef-d7f0-4957-b41c-ce959c73ae5c",
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
              "id": "9be014ed-8828-40d5-b9c1-b759effac7b6"
            }
          ]
        },
        {
          "id": "c0bcd471-cfe2-4e27-8a6d-cb7639df6056",
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
              "id": "16b53b29-7d75-4ecd-aa28-5aa121b8e0e2"
            }
          ]
        },
        {
          "id": "146497c1-0f9e-4f9d-8d39-93c19ceb7d71",
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
              "id": "253b6f51-7617-44d6-ba7e-495ecc9461c1"
            }
          ]
        }
      ]
    }
  ]
}