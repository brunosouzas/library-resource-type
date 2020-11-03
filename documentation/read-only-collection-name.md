# Overview
Use when the resource is specific to get the collection with specific name.

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

## Response
content-type: application/json
HTTP: 200

## Response Error
[response-error](link para pagina de erro)