# Overview
Library with all resource-types to use in your API.

## Resouce-types
  - [create-only-item](link)
  - [crud](link)
  - [delete-only-item](link)
  - [partial-update-only-item](link)
  - [read-only-collection-name](link)
  - [read-only-collection](link)
  - [read-only-file](link)
  - [read-only-item](link)
  - [read-only-paged-collection](link)
  - [update-only-item](link)

### Resource-Type embedded
**errorType**
[responseError](link)
- 504: timeOut
- 503: service Unavailable
- 502: bad Gateway
- 500: internal Server Error
- 429: too Many Requests
- 422: unprocessable Entity
- 415: unsupported Media Type
- 407: proxy Authentication Required
- 406: not Acceptable
- 405: method Not Allowed
- 404: not Found
- 403: forbidden
- 401: not Authorization
- 400: bad Request

**read-only-paged-collection - Use the trait-pageable fragment**
[pageable](link)
- paginated : trait-pageable fragment

## How to use
Import the fragment in your API and add in main raml file or in a library

### Resource type as file

```
resourceTypes:
  read-only-paged-collection: !include exchange_modules/[YOUR ORGANIZATION]/library-resource-typ/[FRAGMENT VERSION]/resourceType/read-only-paged-collection.raml

types:
  error: !include exchange_modules/[YOUR ORGANIZATION]/library-error/[FRAGMENT VERSION]/types/error-eapi.raml

traits:
  paginated: !include exchange_modules/[YOUR ORGANIAZTION]/trait-pageable/[FRAGMENT VERSION]/pageable.raml

/pagination:
  type:
    read-only-paged-collection:
      displayName: paged collection from customer
      errorType: error
      collectionName: customers
      collectionType: customer
      collectionExample: !include examples/customers-pagination.json
      maxItems: 100
```

### Resource type as library
```
uses:
  resourceType: exchange_modules/[YOUR ORGANIZATION]/library-resource-type/[FRAGMENT VERSION]/resource-type.raml

types:
  error: !include exchange_modules/[YOUR ORGANIZATION]/library-error/[FRAGMENT VERSION]/types/error-log.raml

/customers:
  securedBy: security.token
  type:
    resourceType.create-only-item:
      displayName: create a customer
      errorType: error
      inputType: customer
      inputExample: !include examples/customer.json
      outputType: customer
      outputExample: !include examples/customer.json
```