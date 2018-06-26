---
name: NetLicensing
x-slug: netlicensing
description: Labs64 NetLicensing is a first-class solution in the Licensing-as-a-Service
  (LaaS) sector. Based on open standards, it provides a cost effective, integrated
  and scalable platform for software vendors and developers who want to concentrate
  on their product&rsquo;s core functionality instead of spending resources on developing
  an own license management software.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
x-kinRank: "7"
x-alexaRank: "1080577"
tags: NetLicensing
created: "2018-06-26"
modified: "2018-06-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/apis.md
specificationVersion: "0.14"
apis:
- name: NetLicensing Licenses list
  x-api-slug: netlicensing
  description: Return a list of all licenses for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//license
  tags: License
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/license-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/license-get-openapi.md
- name: NetLicensing Create license
  x-api-slug: netlicensing
  description: Creates a new license
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//license
  tags: License
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/license-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/license-post-openapi.md
- name: NetLicensing Delete license
  x-api-slug: netlicensing
  description: Delete license by a licenseNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//license/{licenseNumber}
  tags: License,LicenseNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-delete-openapi.md
- name: NetLicensing Get license
  x-api-slug: netlicensing
  description: Get license by a licenseNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//license/{licenseNumber}
  tags: License,LicenseNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-get-openapi.md
- name: NetLicensing Update license
  x-api-slug: netlicensing
  description: Update license by a licenseNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//license/{licenseNumber}
  tags: License,LicenseNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenselicensenumber-post-openapi.md
- name: NetLicensing Licensees list
  x-api-slug: netlicensing
  description: Return a list of all licensees for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee
  tags: Licensee
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensee-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensee-get-openapi.md
- name: NetLicensing Create licensee
  x-api-slug: netlicensing
  description: Creates a new licensee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee
  tags: Licensee
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensee-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensee-post-openapi.md
- name: NetLicensing Delete licensee
  x-api-slug: netlicensing
  description: Delete a licensee by number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}
  tags: Licensee,LicenseeNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-delete-openapi.md
- name: NetLicensing Get licensee
  x-api-slug: netlicensing
  description: Return a licensee by licenseeNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}
  tags: Licensee,LicenseeNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-get-openapi.md
- name: NetLicensing Update licensee
  x-api-slug: netlicensing
  description: Sets the provided properties to a licensee. Return an updated licensee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}
  tags: Licensee,LicenseeNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumber-post-openapi.md
- name: NetLicensing Transfer licenses
  x-api-slug: netlicensing
  description: Licenses transfer between licensees
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}/transfer
  tags: Licensee,LicenseeNumber,Transfer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbertransfer-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbertransfer-post-openapi.md
- name: NetLicensing Validate licensee
  x-api-slug: netlicensing
  description: Validates active licenses of the licensee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}/validate
  tags: Licensee,LicenseeNumber,Validate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbervalidate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbervalidate-post-openapi.md
- name: NetLicensing License Templates list
  x-api-slug: netlicensing
  description: Return a list of all license templates for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensetemplate
  tags: Licensetemplate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplate-get-openapi.md
- name: NetLicensing Create license template
  x-api-slug: netlicensing
  description: Creates a new license template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensetemplate
  tags: Licensetemplate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplate-post-openapi.md
- name: NetLicensing Delete license template
  x-api-slug: netlicensing
  description: Delete a license template by number.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensetemplate/{licenseTemplateNumber}
  tags: Licensetemplate,LicenseTemplateNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-delete-openapi.md
- name: NetLicensing Get license template
  x-api-slug: netlicensing
  description: Return a license template by licenseTemplateNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensetemplate/{licenseTemplateNumber}
  tags: Licensetemplate,LicenseTemplateNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-get-openapi.md
- name: NetLicensing Update license template
  x-api-slug: netlicensing
  description: Sets the provided properties to a license template. Return an updated
    license template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensetemplate/{licenseTemplateNumber}
  tags: Licensetemplate,LicenseTemplateNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licensetemplatelicensetemplatenumber-post-openapi.md
- name: NetLicensing Payment Methods list
  x-api-slug: netlicensing
  description: Return a list of all payment methods for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//paymentmethod
  tags: Paymentmethod
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethod-get-openapi.md
- name: NetLicensing Get payment method
  x-api-slug: netlicensing
  description: Return a payment method info by paymentMethodNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//paymentmethod/{paymentMethodNumber}
  tags: Paymentmethod,PaymentMethodNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethodpaymentmethodnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethodpaymentmethodnumber-get-openapi.md
- name: NetLicensing Update payment method
  x-api-slug: netlicensing
  description: Sets the provided properties to a payment method. Return an updated
    payment method
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//paymentmethod/{paymentMethodNumber}
  tags: Paymentmethod,PaymentMethodNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethodpaymentmethodnumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/paymentmethodpaymentmethodnumber-post-openapi.md
- name: NetLicensing Products list
  x-api-slug: netlicensing
  description: Return a list of all configured products for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//product
  tags: Product
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/product-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/product-get-openapi.md
- name: NetLicensing Create product
  x-api-slug: netlicensing
  description: Creates a new product
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//product
  tags: Product
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/product-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/product-post-openapi.md
- name: NetLicensing Delete product
  x-api-slug: netlicensing
  description: Delete a product by number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//product/{productNumber}
  tags: Product,ProductNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-delete-openapi.md
- name: NetLicensing Get product
  x-api-slug: netlicensing
  description: Return a product by productNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//product/{productNumber}
  tags: Product,ProductNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-get-openapi.md
- name: NetLicensing Update product
  x-api-slug: netlicensing
  description: Sets the provided properties to a product. Return an updated product
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//product/{productNumber}
  tags: Product,ProductNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productproductnumber-post-openapi.md
- name: NetLicensing Product Modules list
  x-api-slug: netlicensing
  description: Return a list of all product modules for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//productmodule
  tags: Productmodule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmodule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmodule-get-openapi.md
- name: NetLicensing Create product module
  x-api-slug: netlicensing
  description: Creates a new product module
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//productmodule
  tags: Productmodule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmodule-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmodule-post-openapi.md
- name: NetLicensing Delete product module
  x-api-slug: netlicensing
  description: Delete a product module by number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//productmodule/{productModuleNumber}
  tags: Productmodule,ProductModuleNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-delete-openapi.md
- name: NetLicensing Get product module
  x-api-slug: netlicensing
  description: Return a product module by productModuleNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//productmodule/{productModuleNumber}
  tags: Productmodule,ProductModuleNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-get-openapi.md
- name: NetLicensing Update product module
  x-api-slug: netlicensing
  description: Sets the provided properties to a product module. Return an updated
    product module
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//productmodule/{productModuleNumber}
  tags: Productmodule,ProductModuleNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/productmoduleproductmodulenumber-post-openapi.md
- name: NetLicensing Tokens list
  x-api-slug: netlicensing
  description: Return a list of all tokens for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//token
  tags: Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/token-get-openapi.md
- name: NetLicensing Create token
  x-api-slug: netlicensing
  description: Create token by tokenType and additional token parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//token
  tags: Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/token-post-openapi.md
- name: NetLicensing Delete token
  x-api-slug: netlicensing
  description: Delete a token by number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//token/{tokenNumber}
  tags: Token,TokenNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/tokentokennumber-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/tokentokennumber-delete-openapi.md
- name: NetLicensing Get token
  x-api-slug: netlicensing
  description: Return a token by tokenNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//token/{tokenNumber}
  tags: Token,TokenNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/tokentokennumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/tokentokennumber-get-openapi.md
- name: NetLicensing Transactions list
  x-api-slug: netlicensing
  description: Return a list of all transactions for the current vendor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//transaction
  tags: Transaction
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transaction-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transaction-get-openapi.md
- name: NetLicensing Create transaction
  x-api-slug: netlicensing
  description: Creates a new transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//transaction
  tags: Transaction
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transaction-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transaction-post-openapi.md
- name: NetLicensing Get transaction
  x-api-slug: netlicensing
  description: Return a transaction by transactionNumber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//transaction/{transactionNumber}
  tags: Transaction,TransactionNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transactiontransactionnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transactiontransactionnumber-get-openapi.md
- name: NetLicensing Update transaction
  x-api-slug: netlicensing
  description: Sets the provided properties to a transaction. Return an updated transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//transaction/{transactionNumber}
  tags: Transaction,TransactionNumber
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transactiontransactionnumber-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/transactiontransactionnumber-post-openapi.md
- name: NetLicensing License Types list
  x-api-slug: netlicensing
  description: Return a list of all license types supported by the service
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//utility/licenseTypes
  tags: Utility,LicenseTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/utilitylicensetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/utilitylicensetypes-get-openapi.md
- name: NetLicensing Licensing Models list
  x-api-slug: netlicensing
  description: Return a list of all licensing models supported by the service
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//utility/licensingModels
  tags: Utility,LicensingModels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/utilitylicensingmodels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/utilitylicensingmodels-get-openapi.md
- name: NetLicensing Validate licensee
  x-api-slug: netlicensing
  description: Validates active licenses of the licensee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest//licensee/{licenseeNumber}/validate
  tags: Licensee,LicenseeNumber,Validate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbervalidate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/licenseelicenseenumbervalidate-get-openapi.md
- name: NetLicensing
  x-api-slug: netlicensing
  description: Labs64 NetLicensing is a first-class solution in the Licensing-as-a-Service
    (LaaS) sector. Based on open standards, it provides a cost effective, integrated
    and scalable platform for software vendors and developers who want to concentrate
    on their product&rsquo;s core functionality instead of spending resources on developing
    an own license management software.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28466-labs64-net-licensing-restful-api-test-center.jpg
  humanURL: http://netlicensing.io
  baseURL: https://go.netlicensing.io//core/v2/rest
  tags: NetLicensing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/netlicensing/master/_listings/netlicensing/openapi.md
x-common:
- type: x-getting-started
  url: https://netlicensing.io/getting-started/
- type: x-pricing
  url: https://netlicensing.io/pricing/
- type: x-twitter
  url: https://twitter.com/netlicensing
- type: x-website
  url: http://netlicensing.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---