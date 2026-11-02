# SSRF & LFI – Exercise 02

## Overview
This project demonstrates SSRF and Local File Read vulnerabilities in a Flask web application.

## Vulnerabilities
- *SSRF:* The application fetches user-supplied URLs without proper validation, allowing requests to internal services.
- *Local File Read (LFI-related):* The application reads arbitrary local files using file:// URLs without access restrictions.

## Exploitation Scenarios
1. *Local File Disclosure:* Using file:///etc/passwd to read sensitive server files.
2. *Internal Service Access:* Using http://127.0.0.1:5000/ to access the application's internal HTTP endpoint.

## Results
Both tests succeeded, demonstrating unauthorized file reading and unrestricted server-side requests.

## Prevention
Validate URLs, restrict allowed protocols and destinations, block internal addresses, and prevent arbitrary local file access.

Detailed payloads and fixes are documented in Payloads.md and Fix.md.
