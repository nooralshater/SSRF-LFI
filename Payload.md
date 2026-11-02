# SSRF & Local File Read Payloads

## 1. Local File Read

Payload:
file:///etc/passwd

Result:
Successfully displayed the contents of /etc/passwd.

Vulnerability:
The application allows unrestricted access to local server files.

## 2. SSRF

Payload:
http://127.0.0.1:5000/

Result:
Successfully fetched the application's internal homepage.

Vulnerability:
The server accepts user-controlled URLs without restricting internal destinations.

## Conclusion
Both payloads successfully demonstrated SSRF and unauthorized local file reading.
