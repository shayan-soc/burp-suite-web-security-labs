 Lab 02 — Burp Suite Repeater: HTTP Request and Response Analysis

 1. Lab Information

| Field | Details |
|---|---|
| Lab ID | LAB-02 |
| Project | Burp Suite Web Security Labs |
| Tool | Burp Suite Community Edition |
| Version | 2026.10.1 |
| Operating System | Windows 11 |
| Target | https://example.com |
| Difficulty | Beginner |
| Testing Type | HTTP Request and Response Analysis |

 2. Objective

The objective of this lab is to understand HTTP request and response analysis using Burp Suite Proxy and Repeater.

The exercise focuses on capturing an HTTP request, sending it to Repeater, and reviewing the server response.

 3. Tools Used

- Burp Suite Community Edition
- Burp Proxy
- Proxy HTTP History
- Burp Repeater
- Burp's built-in browser

 4. Methodology

1. Opened the target website using Burp's built-in browser.
2. Captured the HTTP traffic using Proxy HTTP History.
3. Identified the request associated with example.com.
4. Sent the selected request to Burp Repeater.
5. Resent the request using the Send button.
6. Compared the response body and inspected HTTP response details.

 5. Findings and Observations

# F-01: HTTP Request Method

Observed value: `GET`

The GET method was used to request a resource from the web server.

# F-02: HTTP Response Status

Initial Proxy observation: `200 OK`

The initial request received a successful HTTP response.

Repeater status verification: To be confirmed from the saved Repeater response evidence.

 # F-03: Target Host

Observed value: `example.com`

The Host header identifies the requested hostname.

# F-04: Response Content Type

Observed value: `text/html; charset=utf-8`

The server response was identified as HTML content using UTF-8 character encoding.

# F-05: Repeater Response Comparison

The response body appeared similar to the response observed in Proxy HTTP History.

The same request was resent without intentional modifications.

This observation does not establish a security vulnerability.

# F-06: Cache Age Header Observation

Values observed: `5975` and `6651`

The exact location of these values requires confirmation from the saved response-header evidence.

If these values were present in the HTTP Age response header, they represent cache-age information in seconds.

No vulnerability is established by this observation.

 6. Proxy vs Repeater

| Proxy HTTP History | Repeater |
|---|---|
| Records captured HTTP traffic | Manually resends selected requests |
| Helps review browser requests | Helps perform controlled request testing |
| Useful for traffic investigation | Useful for response comparison |

 7. Evidence

The following screenshots are included:

1. Proxy HTTP History
2. Repeater Request
3. Repeater Response
4. Response Headers

 8. Conclusion

This lab provided practical experience with HTTP request capture and response analysis using Burp Suite Community Edition.

I practiced identifying HTTP methods, status codes, Host headers, Content-Type headers, and response bodies.

I also learned the difference between Proxy HTTP History and Repeater.

No security vulnerability was confirmed during this exercise.

 9. Security and Ethical Considerations

This exercise involved basic HTTP observation of example.com.

Further security testing will only be conducted on systems I own, intentionally vulnerable training environments, or targets for which I have explicit authorization and permission within the defined scope.

 10. Skills Practiced

- HTTP Request Analysis
- HTTP Response Analysis
- Burp Proxy
- Burp Repeater
- Response Header Inspection
- Evidence Collection
- Technical Documentation
