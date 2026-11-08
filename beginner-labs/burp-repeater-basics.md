# Lab 02 — Learning Notes: Burp Suite Repeater

 1. What is an HTTP Request?

An HTTP request is a message sent by a client, such as a web browser, to a web server.

Example:

```http
GET / HTTP/2
Host: example.com
```

 2. What is an HTTP Response?

An HTTP response is the server's reply to a client's request.

Example:

```http
HTTP/2 200 OK
Content-Type: text/html; charset=utf-8
```

 3. What is Burp Proxy?

Burp Proxy allows a security tester to intercept and inspect HTTP traffic between a browser and a web application.

HTTP History stores a record of captured traffic.

 4. What is Burp Repeater?

Burp Repeater allows a tester to manually resend an HTTP request.

A tester can modify request details and compare the resulting server responses.

 5. Proxy vs Repeater

- Proxy HTTP History: Captures and records traffic.
- Repeater: Manually resends and tests individual requests.

 6. Important HTTP Concepts

| Concept | Meaning |
|---|---|
| GET | Requests a resource |
| POST | Submits data |
| 200 OK | Successful HTTP response |
| 404 Not Found | Requested resource not found |
| Host | Requested hostname |
| Content-Type | Describes response media type |
| Response Body | Main response content |
| Response Headers | Response metadata |
| Age | Cache-related response header, when present |

 7. Practical Workflow

1. Open a website in Burp's browser.
2. Navigate to Proxy HTTP History.
3. Select an HTTP request.
4. Choose Send to Repeater.
5. Open the Repeater tab.
6. Inspect the request.
7. Click Send.
8. Inspect the response status, headers, and body.
9. Record observations.

 8. Learning Outcome

I learned how to capture, inspect, and manually resend HTTP requests using Burp Suite Community Edition.

 9. Safety Rule

Only test systems that I own, authorized training labs, or targets explicitly included in an approved security-testing scope.
