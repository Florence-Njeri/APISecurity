# Mitigating API Security Threats

## Authentication

Only authorized people can access an API.
-Use tokens and API keys

## Authorization

Ensures people only get access to the data they are authorized to access. No overexposure.

## Encryption and signatures

Encryptions protects the data in transit to and from the DB via the API. This ensures integrity of the data in the transit.

## Hashing

## Rate limiting

Limiting the number of requests that can be made to an API over a period of time and keep track of the use history over time. Keeping track of the requests will help you identify an attack if the quota usage gets higher than normal and multiple requests from the same IP within a short timeframe. This helps prevent DDOS or an attacker using an automation tool and brute force to crack a users login credentials.

## Input validation

Most web and mobile applications have some form of form that the user can fill to create or update data in the apps database. Input validation ensures that the data input by the user is safe and an attacker can't add a piece of SQL code that would alter your database. This prevents SQL attacks.

## Add an API gateway
