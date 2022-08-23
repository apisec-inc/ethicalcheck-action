
# APIsec EthicalCheck - Continuous API Security Testing

EthicalCheck addresses the critical need to continuously security test APIs in development and in production.

EthicalCheck provides the industry’s only free & automated API security testing service that uncovers security vulnerabilities using OWASP API list. Developers relies on EthicalCheck to evaluate every update and release, ensuring that no APIs go to production with exploitable vulnerabilities.

You develop the application and API, we bring complete and continuous security testing to you, accelerating development. 

Know your API and Applications are secure with EthicalCheck – our free & automated API security testing service. 

## How EthicalCheck works?
EthicalCheck functions in the following simple steps.

### Security Testing
Provide your OpenAPI specification or start with a public Postman collection URL. EthicalCheck instantly instrospects your API and creates a map of API endpoints for security testing.

It then automatically creates hundreds of security tests that are non-intrusive to comprehensively and completely test for authentication, authorizations, and OWASP bugs your API. The tests addresses the OWASP API Security categories including OAuth 2.0, JWT, Rate Limit etc.

### Reporting

EthicalCheck generates security test report that includes all the tested endpoints, coverage graph, exceptions, and vulnerabilities. Vulnerabilities are fully triaged, it contains CVSS score, severity, endpoint information, and OWASP tagging.

___

## Inputs

### `oas-url`
**Required** The OpenAPI Specification URL or Swagger Path or Public Postman collection URL.

Example OpenAPI Specification URL: http://netbanking.apisec.ai:8080/v2/api-docs

Example Postman Collection URL: https://www.getpostman.com/collections/42d092251d3ae0bea4d4

|Default value|`""`|
--- | ---

### `email`
**Required** The email address to which the penetration test report will be sent.
|Default value|`""`|
--- | ---

## Example (OpenAPI Spec)

```yaml
- name: EthicalCheck - Free & Automated API Security Testing Service
  id: scan
  uses: apisec-inc/ethicalcheck-action@latest
  with:
    oas-url: http://netbanking.apisec.ai:8080/v2/api-docs
    email: xxx@apisec.ai
```

## Example (Postman Collection)

```yaml
- name: EthicalCheck - Free & Automated API Security Testing Service
  id: scan
  uses: apisec-inc/ethicalcheck-action@latest
  with:
    oas-url: https://www.getpostman.com/collections/42d092251d3ae0bea4d4
    email: xxx@apisec.ai
```
