# Overview
Use when the resource is specific to get a paginated collection.

ps. add a traits with 'paginated' name using trait-pageable fragment in your project.

## Method 
GET

## Required Field
- **displayName**
  - display name to method

- **errorType**
  - [error](link para pagina de erro)

- **collectionName**
  - object name to return in your response, example bellow: 
    ```
    {
      customer: []
    }
    ```

- **collectionType**
  - output collection data type

- **collectionExample**
  - output collection example (.json/.raml)

- **maxItems**
  - max items used in paginated

## Response
content-type: application/json
HTTP: 200

## Response Error
[response-error](link para pagina de erro)