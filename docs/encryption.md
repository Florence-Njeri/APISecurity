# Encrypting API requests and responses using SSL/TLS

## Using encryption and digital signatures

**Encryptions** protects the data in storage and transit to and from the DB via the API. This ensures *integrity* of the data in storage as well as the data in transit. Encryption provides *confidentiality*. You can use either asymetric or symetric encryption depending on your needs.

**Digital signatures** on the other hand ensure *data intergrity* of the data in transit to assure the receiver that the data has not been tampered. You use hashing algorthms to sign the data and the receiver will use your public key to hash the message they received. If the original hash message and the recepient hash message are a match, then the senders authenticity is assured. This will help mitigate man in the **middle attacks**.
