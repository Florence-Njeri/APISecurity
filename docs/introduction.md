# Introduction to API Security

API is which is short for Application Programming Interface, is an intermediary that allows two or more applications to communicate with each other. If an application e.g Twitter has an API, then external/third party clients can use it to make requests. APIs often provide the capability to create, read and modify sensitive information stored in an organization. If the third parties accessing an API manage to get hold of sensitive information about an application or the people using the app, this may lead to a **data breach**.

API security on the other hand is the process and the measures put in place to protect APIs and the data read, created or updated by these APIs from security attacks. Since the applications expose their APIs to the public, the APIs are at a bigger risk of exploitation of vulnerabilities to gain unauthorized access which compromized the integrity and confidentiality aspect of the data transimitted by your APIs.

## Common API security risks

### Authentication-based attacks

Authentication and session management
Most APIs require the users to get authenticated before they can sytart making requests. However, there are several ways an attacker could compromise this e.g by social engineering or phishing to obtain the users authentication credentials or even intercepting the token returned when the user logs in. If the API has excessive data returned in the token, then the attacker will be able to access users data.

After a user is authenticated, most application retain some data refred to as session data for subsequent requests authentication which containst information such as a users access rights.

Example:

### Authorization errors

Authorization dictates the level of access a user has. If not carefully managed, a user may end up having access to more data than they need and in the instance that their account gets compromised, the applications has a wider risk.

Example:

### DDOS attacks

An attacker can automate the brute force method they use to try login to your application. Too many requests targeted towards the API may make the API unavailable to authentic users of your API.

Example:

### SQL injection attacks

An SQL injection mostly happens when forms and API requests don't validate user input to reject code as input. If the app doesn't validate user input before the data is added to its database, the SQL queries may be manipulated by the code the attacker puts in to manipulate the users database e.g to add a backdoor to the app or even delete or manipulate records in the db.

The APIs are basically querying the database.

Example: https://blog.shiftleft.io/api-security-101-injection-a7feea1d4fd

### Insecure direct object refences (IDOR)

IDOR is an API vulnerability from the lack of access rights in an applications. Using IDOR, an attacker can manipulate the direct object reference such as a URL query parameter, database key, session id etc and get acess to data or information they shouldn't be able to access. For example, if your bank includes your user id in the URL you use to access your banking information, an attacker can try and change the id to another users id and if the applications hasn't enforced authorization checks, the attacker will be able to get access to other users banking details. Even worse is if they are able to use an automation tool to loop through all the users in the application and access their data. In this scenario, the user id is the direct object reference.

Using IDOR an attacker can access data they aren't authorized to access. This is one case of excessive data exposure in applications.

Example:


### Cross-site scripting (XSS) attacks

