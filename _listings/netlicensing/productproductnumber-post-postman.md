{
  "info": {
    "name": "NetLicensing Update product",
    "_postman_id": "8db8dcd9-6103-47a0-b9f3-5981bd520f37",
    "description": "Sets the provided properties to a product. Return an updated product",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "License",
      "item": [
        {
          "id": "73a49d3d-d407-4225-80b5-dcb2bd7e2b76",
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
              "id": "57988ea6-3b09-4b42-b67d-6c6cf9c57d3c"
            }
          ]
        },
        {
          "id": "0dd3051d-00ca-400e-b04f-be7b10fc3301",
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
              "id": "081a6e84-2745-447a-88d3-b10a9d1f1a1c"
            }
          ]
        },
        {
          "id": "dea53d75-0f2e-4457-83c4-ba378d251fa0",
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
              "id": "bef03041-2bde-496e-998b-67e995d67b3d"
            }
          ]
        },
        {
          "id": "29db4079-dd29-4540-aac8-92487fe12cce",
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
              "id": "137cb6b9-495d-43e5-bdc8-8517cf1031d7"
            }
          ]
        },
        {
          "id": "e41c4c29-7529-46ef-8959-9aa4866d91c5",
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
              "id": "9f40487b-dff5-4c86-83fd-476609283245"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensee",
      "item": [
        {
          "id": "bcd3b5cf-c5bf-4846-967e-e0f41200d521",
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
              "id": "47c1bffa-ce80-4c6a-87af-b338708717e1"
            }
          ]
        },
        {
          "id": "7acfd727-0802-443f-af6d-806bf4472edb",
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
              "id": "5cd4e136-b0ab-4a3a-82b8-5119baf94f82"
            }
          ]
        },
        {
          "id": "5d7db591-b6c5-4a17-b756-ab51b67c407b",
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
              "id": "f0fcff95-6a44-4f2c-9e88-a499b6858187"
            }
          ]
        },
        {
          "id": "467b12a2-047d-4e6a-9715-b4ffd288a0c2",
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
              "id": "2bb312c3-2802-4fa3-a400-e35cef626b24"
            }
          ]
        },
        {
          "id": "33dc1a4e-643c-45b9-a971-f4db9abbd165",
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
              "id": "a5b67651-44e9-414f-84e2-672d8103d38c"
            }
          ]
        },
        {
          "id": "4047a4e9-405e-4e28-ad1b-f2cc818fabf3",
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
              "id": "4083c0be-c433-4ce1-9444-02bb9bda14fc"
            }
          ]
        },
        {
          "id": "dd8b434e-faf9-4dfb-b103-136018d49e67",
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
              "id": "49238a78-f752-4233-ae19-15768edf5b32"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensetemplate",
      "item": [
        {
          "id": "6f75d0c3-e85c-4f8c-9792-d28cd645c265",
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
              "id": "e6421461-e378-4b29-a0ce-e2069e3846ae"
            }
          ]
        },
        {
          "id": "e7ca74f3-ec16-4874-b986-9393586b3206",
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
              "id": "8225e29e-ce76-4000-ba52-6056612c0e87"
            }
          ]
        },
        {
          "id": "50f8649f-888a-4580-8af1-ebfde69081e1",
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
              "id": "39fec0f5-a6d1-4ae7-8a7a-18826af84ff5"
            }
          ]
        },
        {
          "id": "deba409d-c82a-43e1-81e6-c2ba100eabbb",
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
              "id": "156593b5-cf80-4933-96f2-a4a3e002ce95"
            }
          ]
        },
        {
          "id": "8d3aac75-89c5-45c6-a300-f86c54b149e3",
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
              "id": "27e4ea8c-388e-47e7-89b6-bbdf5a5711b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "429a548b-5f37-43d9-b9f1-709de05b2c2e",
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
              "id": "31b47da7-1fbe-404b-96a8-fe1cf8858b97"
            }
          ]
        },
        {
          "id": "7414ea14-5ad4-4fc6-8f63-40df399cffed",
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
              "id": "690d2c82-c0ff-44ac-9cbd-61a8c5d2137c"
            }
          ]
        },
        {
          "id": "19388c74-ebb7-4e3b-8878-13073abc2041",
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
              "id": "008d9a66-965a-4825-8f29-10fc508b3c75"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "5cd74581-6b14-4418-a2c7-dffce6f67ead",
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
              "id": "51f27fd3-5b18-4cf8-9722-071f51e4ef53"
            }
          ]
        },
        {
          "id": "110ead9b-0809-4868-97b0-889f3bbee428",
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
              "id": "384fff25-a552-40f1-8c97-da31c5fe7d86"
            }
          ]
        },
        {
          "id": "0818160c-9145-4ba7-8a30-1af89421430a",
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
              "id": "c0694cd3-4de2-4b0d-a7e0-566cf3ba235f"
            }
          ]
        },
        {
          "id": "7ce8232a-f5f6-43b9-82a7-140e38096eb6",
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
              "id": "ac98e008-6f60-40be-92e9-5c60c47692d6"
            }
          ]
        },
        {
          "id": "e798ff07-cd2e-411f-b04a-c50a3d229671",
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
              "id": "117f2af0-cea2-430d-a1a1-2b9876f1437b"
            }
          ]
        }
      ]
    }
  ]
}