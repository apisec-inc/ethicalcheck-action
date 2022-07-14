[![APIsec](https://cloud.fxlabs.io/assets/images/logo.png)](https://www.apisec.ai/product)

APIsec addresses the critical need to secure APIs before they reach production. APIsec provides the industry’s only automated and continuous API testing platform that uncovers security vulnerabilities and logic flaws in APIs. Clients rely on APIsec to evaluate every update and release, ensuring that no APIs go to production with vulnerabilities.

You develop the application and API, we bring complete and continuous security testing to you, accelerating development. 

Know your API and Applications are secure with Apisec – our automated and continuous API security testing platform. 

## How Apisec Free Pentest works:
Apisec functions in the following simple steps.

### API Scanning
Provide your  OpenAPI specification URL. Apisec instantly learns your live API composition, including the list of endpoints and operations, and creates an API functionality map.

Apisec automatically creates thousands of attack playbooks to comprehensively and completely test every function of your API. The playbooks address the entire OWASP API Security Top 10 and more, giving you complete coverage.

Apisec runs non-intrusive scan/playbooks against your APIs to find the vulnerabilities.

### Vulnerabilities Reporting
The Apisec playbooks are designed to find the trickiest vulnerabilities - business logic flaws, OWASP API top 10, and not just standard security issues. 

APIsec sends Pentest Report with OWASP Coverage, Category wise Test Cases and Vulnerabilities count to the email provided.

___

## Inputs

### `oas-url`
**Required** The Open API Specification URL against which the scans will be executed.

|Default value|`""`|
--- | ---

### `email`
**Required** The email address on which the vulnerabilities report will be sent.
|Default value|`""`|
--- | ---

## Example usage

```yaml
- name: Trigger APIsec Free Pen Test
  id: scan
  uses: apisec-inc/apisec-free-pentest@latest
  with:
    oas-url: http://netbanking.apisec.ai:8080/v2/api-docs
    email: xxx@apisec.ai
```
