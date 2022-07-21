[![APIsec](https://cloud.fxlabs.io/assets/images/logo.png)](https://www.apisec.ai/product)

EthicalCheck addresses the critical need to secure APIs before they reach production. EthicalCheck provides the industry’s only free & instant API penetration testing service that uncovers security vulnerabilities and OWASP API list in APIs. Dev relies on EthicalCheck to evaluate every update and release, ensuring that no APIs go to production with vulnerabilities.

You develop the application and API, we bring complete and continuous security testing to you, accelerating development. 

Know your API and Applications are secure with EthicalCheck – our free & instant API penetration testing service. 

## How EthicalCheck works?
EthicalCheck functions in the following simple steps.

### Security Testing
Provide your OpenAPI specification or public Postman collection URL. EthicalCheck instantly instrospects your API and creates a map of API endpoints for security testing.

It then automatically creates hundreds of security tests that are non-intrusive to comprehensively and completely test every attack surface of your API. The tests addresses the OWASP API Security categories including OAuth 2.0, JWT, Rate Limit, CORS etc.

### Reporting

EthicalCheck generates penetration test report that includes all the tested endpoints, coverage graph, exceptions, and vulnerabilities. Vulnerabilities are fully triaged, it contains CVSS score, severity, endpoint information, and OWASP tagging.

___

## Inputs

### `oas-url`
**Required** The Open API Specification or Public Postman collection URL.

|Default value|`""`|
--- | ---

### `email`
**Required** The email address to which the penetration test report will be sent.
|Default value|`""`|
--- | ---

## Example usage

```yaml
- name: EthicalCheck - Free & Instant API Penetration Testing Service
  id: scan
  uses: apisec-inc/apisec-free-pentest@latest
  with:
    oas-url: http://netbanking.apisec.ai:8080/v2/api-docs
    email: xxx@apisec.ai
```
