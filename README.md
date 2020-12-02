# micronaut_jwt_security

Token : \
eyJhbGciOiJIUzUxMiJ9.eyJqdGkiOiIyMzUxMjM1MTM0NTQxMyIsImlzcyI6IkRETSIsImV4cCI6MTcwNjgzNzI5OCwiaWF0IjoxNjA2ODM2Mzk4LCJ1c2VyX2lkIjo4MDAsInJvbGVzIjpbIkFETUlOIl0sInVzZXJfZmlyc3RfbmFtZSI6IkFkIiwidXNlcl9sYXN0X25hbWUiOiJNaW4iLCJ1c2VyX2VtYWlsIjoiYWRtaW5Ad2hhdGV2ZXIuY29tIn0.2Ucx1qeEp8qCQNDiX7A513J3DKdrg7XPfVeQbD8wwTH9U-90jHV9COVUiR-XlMqehkJ2e5vRs4BA1jHECFpWDA
Secret : test

<h3>To check</h3>
https://jwt.io/#debugger-io?token=eyJhbGciOiJIUzUxMiJ9.eyJqdGkiOiIyMzUxMjM1MTM0NTQxMyIsImlzcyI6IkRETSIsImV4cCI6MTcwNjgzNzI5OCwiaWF0IjoxNjA2ODM2Mzk4LCJ1c2VyX2lkIjo4MDAsInJvbGVzIjpbIkFETUlOIl0sInVzZXJfZmlyc3RfbmFtZSI6IkFkIiwidXNlcl9sYXN0X25hbWUiOiJNaW4iLCJ1c2VyX2VtYWlsIjoiYWRtaW5Ad2hhdGV2ZXIuY29tIn0.2Ucx1qeEp8qCQNDiX7A513J3DKdrg7XPfVeQbD8wwTH9U-90jHV9COVUiR-XlMqehkJ2e5vRs4BA1jHECFpWDA&setret=test

<h3>Unprotected</h3>
URL : http://127.0.0.1:8080/ping

Code : \
curl --location --request GET 'http://127.0.0.1:8080/ping'

<H3>Protected</h3>
URL : http://127.0.0.1:8080/secret

Code : \
curl --location --request GET 'http://127.0.0.1:8080/secret' \
--header 'Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJqdGkiOiIyMzUxMjM1MTM0NTQxMyIsImlzcyI6IkRETSIsImV4cCI6MTcwNjgzNzI5OCwiaWF0IjoxNjA2ODM2Mzk4LCJ1c2VyX2lkIjo4MDAsInJvbGVzIjpbIkFETUlOIl0sInVzZXJfZmlyc3RfbmFtZSI6IkFkIiwidXNlcl9sYXN0X25hbWUiOiJNaW4iLCJ1c2VyX2VtYWlsIjoiYWRtaW5Ad2hhdGV2ZXIuY29tIn0.2Ucx1qeEp8qCQNDiX7A513J3DKdrg7XPfVeQbD8wwTH9U-90jHV9COVUiR-XlMqehkJ2e5vRs4BA1jHECFpWDA'

