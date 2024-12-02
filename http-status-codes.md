# HTTP Status Codes 📜

This document provides a comprehensive list of **HTTP status codes** and their meanings. These codes are essential for understanding the communication between the **client** and **server**.

## 1xx: Informational 🧠
These status codes indicate that the request has been received and is being processed.

- **100 Continue**: The request has been received, and the client should continue sending the request body. 🔄
- **101 Switching Protocols**: The server is switching to a different protocol as per the client's request. 🔄
- **102 Processing**: The server is processing the request, but no response is available yet. 🕒

## 2xx: Success ✅
These codes indicate that the request was successfully processed.

- **200 OK**: The request was successful, and the server returned the requested resource. 🎉
- **201 Created**: The request was successful, and a new resource has been created. 🌱
- **202 Accepted**: The request has been accepted for processing, but it is not yet complete. ⏳
- **203 Non-Authoritative Information**: The request was successful, but the data returned may be from a third-party source. 📡
- **204 No Content**: The request was successful, but there’s no content to return. 🚫
- **205 Reset Content**: The request was successful, but the client should reset the document view. 🔄
- **206 Partial Content**: The server is delivering part of the requested resource. ⚡

## 3xx: Redirection 🔀
These codes indicate that the client needs to take further action to complete the request, often by following a new URL.

- **300 Multiple Choices**: Multiple possible responses are available; the client can choose one. 🔄
- **301 Moved Permanently**: The resource has been permanently moved to a new URL. 🔗
- **302 Found**: The requested resource is temporarily located at a different URL. 🔄
- **303 See Other**: The client should retrieve the resource from a different URL. 🌐
- **304 Not Modified**: The resource has not been modified since the last request. 🔄
- **305 Use Proxy**: The client must access the resource through a specified proxy. 🔌
- **306 (Unused)**: This code is no longer used. 🚫
- **307 Temporary Redirect**: The resource has been temporarily moved to a new URL. 🔄
- **308 Permanent Redirect**: The resource has permanently moved to a new URL. 🔗

## 4xx: Client Errors ❌
These codes indicate that the request sent by the client was incorrect or invalid.

- **400 Bad Request**: The request could not be understood due to malformed syntax. ⚠️
- **401 Unauthorized**: The client must authenticate to access the requested resource. 🔐
- **402 Payment Required**: This code is reserved for future use. 💸
- **403 Forbidden**: The client does not have permission to access the requested resource. 🚫
- **404 Not Found**: The server could not find the requested resource. 🌍❌
- **405 Method Not Allowed**: The HTTP method used is not allowed for the requested resource. 🛑
- **406 Not Acceptable**: The server cannot generate a response that matches the client’s request. 🚫
- **407 Proxy Authentication Required**: The client must authenticate through a proxy. 🔒
- **408 Request Timeout**: The client took too long to send the request. ⏰
- **409 Conflict**: The request conflicts with the current state of the resource. 🔄
- **410 Gone**: The resource is no longer available and has been permanently removed. 🗑️
- **411 Length Required**: The server requires the `Content-Length` header. 📏
- **412 Precondition Failed**: One of the conditions in the request header was not met. ⚠️
- **413 Payload Too Large**: The request is too large for the server to process. 🚫
- **414 URI Too Long**: The URI in the request is too long for the server to process. 📏
- **415 Unsupported Media Type**: The server cannot process the media type of the request. 🛑
- **416 Range Not Satisfiable**: The requested range is not available in the resource. ❌
- **417 Expectation Failed**: The server cannot meet the requirements of the `Expect` header. ⚠️
- **418 I'm a teapot**: A playful status code from [RFC 2324](https://tools.ietf.org/html/rfc2324), meaning the server is a teapot and cannot brew coffee. 🍵
- **421 Misdirected Request**: The request was directed to a server that cannot produce a response. 🔄
- **422 Unprocessable Entity**: The request is well-formed, but the server cannot process it (e.g., invalid data). ⚠️
- **423 Locked**: The resource is locked and cannot be modified. 🔒
- **424 Failed Dependency**: The request failed due to a failure of a previous request. 🔄
- **425 Too Early**: The server is unwilling to process the request due to a potential replay. ⏳
- **426 Upgrade Required**: The client must upgrade to a different protocol. 🔝
- **428 Precondition Required**: The request requires certain conditions to be met. 🛑
- **429 Too Many Requests**: The client has sent too many requests in a short period. 🚫
- **431 Request Header Fields Too Large**: The headers are too large for the server to process. 📏
- **451 Unavailable For Legal Reasons**: The resource is unavailable for legal reasons (e.g., censorship). ⚖️

## 5xx: Server Errors ⚠️
These codes indicate that the server failed to fulfill a valid request.

- **500 Internal Server Error**: The server encountered an unexpected error. ⚠️
- **501 Not Implemented**: The server does not support the functionality required to fulfill the request. 💻
- **502 Bad Gateway**: The server received an invalid response from an upstream server. 🌐
- **503 Service Unavailable**: The server is temporarily unavailable due to overload or maintenance. 🛠️
- **504 Gateway Timeout**: The server did not receive a timely response from an upstream server. ⏳
- **505 HTTP Version Not Supported**: The server does not support the HTTP version in the request. 🔒
- **506 Variant Also Negotiates**: The server has an internal configuration error. ⚙️
- **507 Insufficient Storage**: The server cannot store the representation needed to complete the request. 💾
- **508 Loop Detected**: The server detected an infinite loop while processing the request. 🔄🔄
- **510 Not Extended**: The server requires further extensions to fulfill the request. ➕
- **511 Network Authentication Required**: The client must authenticate to gain network access. 🔑
