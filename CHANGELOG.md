# Changelog

### Version 0.2.1
- Minor import bugfix for error "'module' object has no attribute 'util'" when using Kerberos delegation on older Python builds

### Version 0.2.0
- Switched core HTTP transport from urllib2 to requests
- Added support for NTLM (via requests_ntlm)
- Added support for kerberos delegation (via requests_kerberos)
- Added support for explicit kerberos principals (in conjuction w/ pykerberos bugfix)
- Timeouts are more configurable

### Version 0.1.1
- Force basic auth header to avoid additional HTTP request and reduce latency
- Python 2.7.9+. Allow server cert validation to be ignored using SSLContext.verify_mode
- Tests. Enable Python 3.4 on Travis CI

### Version 0.0.3

- Use xmltodict instead of not supported xmlwitch
- Add certificate authentication support
- Setup PyPI classifiers
- Fix. Include UUID when sending request
- Fix. Python 2.6.6/CentOS. Use tuples instead of lists in setup.py
- Fix. Python 2.6. String formatting
- Handle unauthorized response and raise UnauthorizeError
- Convert different forms of short urls into full well-formed endpoint
- Add Session.run_ps() helper to execute PowerShell scripts