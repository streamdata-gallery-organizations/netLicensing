{
  "info": {
    "name": "NetLicensing Create token",
    "_postman_id": "f3643620-ea1b-4bdf-b5d1-c8a3380d45b8",
    "description": "Create token by tokenType and additional token parameters",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "License",
      "item": [
        {
          "id": "5f983435-a4cd-4e74-ab18-78b80a161ae5",
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
              "id": "0c87e90d-2a46-4b93-9557-e60b483148fc"
            }
          ]
        },
        {
          "id": "be10c009-6150-418f-afe0-07ca6786e02f",
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
              "id": "804c8276-3f94-475e-adc4-f3375d54b907"
            }
          ]
        },
        {
          "id": "01de39e9-3792-4a2b-a22b-57f4a07e5de7",
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
              "id": "d47054c3-94dc-4a0d-91a1-d4fcdacaa4fc"
            }
          ]
        },
        {
          "id": "3b2a4029-8271-43e2-a9a2-356a1eaddaaa",
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
              "id": "4869840e-2b72-4c3d-a67e-83eaa0778e6d"
            }
          ]
        },
        {
          "id": "86f5bd82-ee5a-4a28-abe8-46a96acf8ad4",
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
              "id": "78006b49-de27-420c-9142-0650a5ce4bc2"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensee",
      "item": [
        {
          "id": "f0e788bc-2acd-4168-a6c4-ed0123c59a8d",
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
              "id": "de054bf0-281c-4261-8aec-4639f4dc0fc5"
            }
          ]
        },
        {
          "id": "42450809-2a46-4133-a0b1-fc6b26e500a3",
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
              "id": "2ddaa3ae-054b-4d8e-8ee9-0746bf681ce9"
            }
          ]
        },
        {
          "id": "b6cb6ceb-de4a-4f11-b11b-cf37b4ea5ab2",
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
              "id": "d0998605-9ef6-4500-b940-f93c10c30736"
            }
          ]
        },
        {
          "id": "334c2f0d-a98f-4bba-9dd3-1ac975ca1f30",
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
              "id": "34293586-5d5b-419c-bed3-30452056be7d"
            }
          ]
        },
        {
          "id": "fd14c635-905b-452c-a80d-22fb53ca8de2",
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
              "id": "b34883c7-48f0-4749-9d6b-3fb0a322bfe1"
            }
          ]
        },
        {
          "id": "dc6f0b14-d3b4-47c9-925e-fa4c013b9803",
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
              "id": "fa0a92b7-f635-4fe8-85ce-19e991462772"
            }
          ]
        },
        {
          "id": "f4e6ebde-0881-4bff-acdb-47e7b8bcdea8",
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
              "id": "9a4c313b-2419-48ce-a8fa-477a3154f404"
            }
          ]
        }
      ]
    },
    {
      "name": "Licensetemplate",
      "item": [
        {
          "id": "fd156010-946e-44c9-ade6-79757114fd59",
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
              "id": "884d94ad-b95d-41b5-afd3-abeefe737401"
            }
          ]
        },
        {
          "id": "ac829654-d59a-4917-ba3f-8a4c4cc6d39b",
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
              "id": "c79f74db-cbe0-4558-83c4-710012108c5b"
            }
          ]
        },
        {
          "id": "2e5d1412-746b-4ebf-8aa9-d15392096534",
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
              "id": "fd22a34d-51b0-49d0-9e67-a7aad90bc436"
            }
          ]
        },
        {
          "id": "31fc0e0b-529d-4c65-854a-f441d3620db1",
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
              "id": "b72da92d-1ce0-42b4-a3dd-f00e35c38b10"
            }
          ]
        },
        {
          "id": "136cef54-1a70-4a30-9011-c0ab5e1f0607",
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
              "id": "15497cf3-4135-414c-8603-1785a0fea28f"
            }
          ]
        }
      ]
    },
    {
      "name": "Paymentmethod",
      "item": [
        {
          "id": "6a40db11-5d4e-402a-b034-65503afbe360",
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
              "id": "c1500960-5cc9-4f66-94d4-c02fba3986ed"
            }
          ]
        },
        {
          "id": "f999bf2c-9d1b-4323-9ef2-5bd36c62bb77",
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
              "id": "b3ad397f-3b9c-4c8e-92b9-ea97b2b90611"
            }
          ]
        },
        {
          "id": "41698258-d5c2-4bd8-8e62-2e8c2aa510df",
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
              "id": "3fe6b140-4064-405f-abf4-18eaf0c7a9e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "be46b991-be62-447a-b89a-823866de4989",
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
              "id": "0934645f-12d3-4ed7-917a-857345c166c0"
            }
          ]
        },
        {
          "id": "2363ef7e-074f-4a21-a870-8f23bc0da7e5",
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
              "id": "2f43bb3a-1be2-4b48-8af4-dcc25bdd0fd6"
            }
          ]
        },
        {
          "id": "898bc344-06ca-4404-92df-9e8fe48d499d",
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
              "id": "e5e99d04-4990-42e4-a6e7-4b0ce21689e5"
            }
          ]
        },
        {
          "id": "cc450a7d-3437-4abf-8b95-aeacc4218e55",
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
              "id": "728ae478-0c64-43be-a611-b261add2475a"
            }
          ]
        },
        {
          "id": "e3d05e99-b36c-42ac-a22a-04bdb9aee31b",
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
              "id": "a143d537-68d0-44f1-bd51-9411b5213da8"
            }
          ]
        }
      ]
    },
    {
      "name": "Productmodule",
      "item": [
        {
          "id": "f208e6b3-acb5-4d3b-be75-fa04b9afb4f8",
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
              "id": "69c8fa77-8a1f-4ce2-8931-caefdefdd136"
            }
          ]
        },
        {
          "id": "55d5d70d-d655-4076-8e6c-1dfeb1dd4a52",
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
              "id": "72e31384-d9a4-4325-a6db-1222a8912a8c"
            }
          ]
        },
        {
          "id": "bce7478c-3e71-4dfa-9853-d5987441d0b0",
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
              "id": "07d68901-e504-4763-bd67-e0f13a1e30e5"
            }
          ]
        },
        {
          "id": "e7314f5a-32a5-4205-8c6d-5e4605a036b8",
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
              "id": "235ea0ba-319c-4197-a4c5-9a61621007a3"
            }
          ]
        },
        {
          "id": "1113a0b8-c079-4954-abf1-4459fdc6deba",
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
              "id": "ea5300c9-e6d5-4fb1-b796-9ef2cd07e554"
            }
          ]
        }
      ]
    },
    {
      "name": "Token",
      "item": [
        {
          "id": "9c657fad-8065-4757-813f-39493b184934",
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
              "id": "0e0da4f3-5c12-443c-92d8-82fd20b88469"
            }
          ]
        },
        {
          "id": "3506548b-be2f-4623-b279-25c15388b199",
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
              "id": "797ca204-6df1-4721-865c-9d80d3e6f551"
            }
          ]
        }
      ]
    }
  ]
}