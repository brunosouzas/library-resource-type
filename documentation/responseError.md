# Overview
Errors used in resourceType

## 504: timeOut
This status code and error message will be returned in case if the proxy timed out waiting for response from service implementation

## 503: service Unavailable
This status code and error message will be returned in case if the server is currently unable to handle the request due to a temporary outage

## 502: bad Gateway
This status code will be returned in case the requested resource received an invalid response from the upstream server.

## 500: internal Server Error
This status code and error message will be returned in case if the API encounters any internal server error and is unable to process the request

## 429: too Many Requests
This status code and error message will be returned in case if within a given duration, the client has made too many requests to the API - hence the rate limiting is applied

## 422: unprocessable Entity
This status code and error message will be returned in case if semantically incorrect entity is provided as input

## 415: unsupported Media Type
This status code and error message will be returned in case if the API encounters any errors like Unsupported media type.

## 407: proxy Authentication Required
This status code and error message will be returned in case if the API requires proxy authentication

## 406: not Acceptable
This status code and error message will be returned in case if the API encounters any errors like Not acceptable.

## 405: method Not Allowed
This status code and error message will be returned in case if the API encounters any errors like Method not allowed.

## 404: not Found
This status code and error message will be returned in case if the API encounters any errors like Resource not found.

## 403: forbidden
This status code and error message will be returned in case if the user is not allowed to perform the requested operation

## 401: not Authorization
This status code and error message will be returned in case if no credentials are provided or the provided credentials are refused

## 400: bad Request
This status code and error message will be returned in case if the API encounters a Bad request.

## 304: not Modified
This status code will be returned in case the requested resource has not been modified since the previous call
