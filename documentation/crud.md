# Overview
Use when the resource is CRUD (POST, GET, PUT, DELETE).

## Create
### Method 
POST

### Required Field
- **displayName**
  - display name to method

- **inputType**
  - input data type

- **inputExample**
  - input example (.json/.raml)

- **errorType**
  - [error](link para pagina de erro)

- **outputType**
  - output data type

- **outputExample**
  - output example (.json/.raml)

### Response
content-type: application/json
HTTP: 201
HTTP: 202

### Response Error
[response-error](link para pagina de erro)

## Read
### Method 
GET

### Required Field
- **displayName**
  - display name to method

- **errorType**
  - [error](link para pagina de erro)

- **collectionType**
  - output collection data type

- **collectionExample**
  - output collection example (.json/.raml)

### Response
content-type: application/json
HTTP: 200

### Response Error
[response-error](link para pagina de erro)

## Partial Update
### Method 
PATCH

### Required Field
- **displayName**
  - display name to method

- **inputType**
  - input data type

- **inputExample**
  - input example (.json/.raml)

- **errorType**
  - [error](link para pagina de erro)

### Response
content-type: application/json
HTTP: 204

### Response Error
[response-error](link para pagina de erro)

## Update
### Method 
PUT

### Required Field
- **displayName**
  - display name to method

- **inputType**
  - input data type

- **inputExample**
  - input example (.json/.raml)

- **errorType**
  - [error](link para pagina de erro)

### Response
content-type: application/json
HTTP: 204

### Response Error
[response-error](link para pagina de erro)

## Delete
### Method 
DELETE

### Required Field
- **displayName**
  - display name to method

- **errorType**
  - [error](link para pagina de erro)

### Response
content-type: application/json
HTTP: 204

### Response Error
[response-error](link para pagina de erro)