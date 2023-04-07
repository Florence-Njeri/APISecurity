# Mitigating API Security Threats

## Authentication and session management

Only authorized people can access an API.
-Use tokens and API keys

## Authorization

Ensures people only get access to the data they are authorized to access. No overexposure.

## Role Based Acccess (RBA)

Implementing RBA which restricts user access to only the data and functionality necessary for their job function. Additionally, APIs can regularly review and update user permissions to ensure that they align with business needs and do not create unnecessary risks. By prioritizing authorization security, organizations can minimize the risk of unauthorized access and protect sensitive data.

## Encryption and signatures

Encryptions protects the data in storage and transit to and from the DB via the API. This ensures integrity of the data in storage as well as the data in transit. Encryption provides confidentiality. Type of encryption to use - assymetric/symetric

## Hashing 

Ensures Confidentiality and Integrity are mainatined.

## Rate limiting

Limiting the number of requests that can be made to an API over a period of time and keep track of the use history over time. Keeping track of the requests will help you identify an attack if the quota usage gets higher than normal and multiple requests from the same IP within a short timeframe. This helps prevent DDOS or an attacker using an automation tool and brute force to crack a users login credentials.

## Input validation

Most web and mobile applications have some form of form that the user can fill to create or update data in the apps database. Input validation ensures that the data input by the user is safe and an attacker can't add a piece of SQL code that would alter your database. This prevents SQL attacks.

## Add an API gateway

## The principle of least priviledge

Grant access on a need to know basis
