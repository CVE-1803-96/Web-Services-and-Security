# Chapter 2: Core Technologies of the Web

## 2.1 HTTP/HTTPS Deep Dive

### HTTP Requests (Methods)
- **GET**: Retrieve data from the server.
- **POST**: Submit data to be processed to the server.
- **PUT**: Update existing data on the server.
- **DELETE**: Remove data from the server.
- Others: HEAD, OPTIONS, PATCH, etc.

### HTTP Responses (Status Codes)
- **200 OK**: The request was successful.
- **201 Created**: A new resource has been created.
- **400 Bad Request**: The request was malformed.
- **401 Unauthorized**: Authentication is required.
- **403 Forbidden**: Access is forbidden.
- **404 Not Found**: The requested resource does not exist.
- **500 Internal Server Error**: Server encountered an error.

### HTTP Headers
- **Content-Type**: Specifies the media type of the resource (e.g., application/json).
- **Authorization**: Credentials for authentication.
- **Cache-Control**: Directives for caching mechanisms.
- **CORS (Cross-Origin Resource Sharing)**: Controls access to resources across different origins.

---

## 2.2 Data Formats for Exchange

### XML (eXtensible Markup Language)
- **Structure**: Hierarchical markup language.
- **Elements**: Defined tags to encapsulate data.
- **Attributes**: Additional information within tags.

### JSON (JavaScript Object Notation)
- **Syntax**: Lightweight, text-based format using key-value pairs.
- **Data Types**: Strings, numbers, objects, arrays, booleans, null.
- **Advantages over XML**:
  - Simpler and more readable.
  - More efficient parsing.
  - Native support in JavaScript.

---

## 2.3 Introduction to TLS/SSL (The "S" in HTTPS)

### Purpose
- **Encryption**: Secures data in transit.
- **Authentication**: Verifies server identity via certificates.
- **Data Integrity**: Ensures data isn't tampered with during transfer.

### High-level Overview of a TLS Handshake
1. **Client Hello**: Client initiates connection, proposes supported cipher suites and protocol versions.
2. **Server Hello**: Server responds, selects cipher suite and protocol, and sends its digital certificate.
3. **Key Exchange**: Client and server generate shared secret keys (via Diffie-Hellman or RSA).
4. **Finished**: Both parties confirm the handshake, encrypted communication begins.
  
This process establishes a secure, encrypted channel between client and server, enabling safe data transmission over HTTPS.
