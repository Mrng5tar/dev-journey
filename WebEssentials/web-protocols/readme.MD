# 🌐 Web Protocols Overview

This section covers the core protocols, standards, and networking concepts that power communication on the modern web. These are fundamental to understanding how browsers and servers exchange data.

---

## 🔐 HTTP vs HTTPS

- **HTTP (HyperText Transfer Protocol)**:

  - Protocol used to transfer web pages.
  - Sends data in plain text (not secure).

- **HTTPS (HTTP Secure)**:

  - Uses SSL/TLS to encrypt communication.
  - Ensures data integrity, privacy, and authentication.

🔗 [MDN – Introduction to HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)

🔗 [Cloudflare – What is HTTPS?](https://www.cloudflare.com/learning/ssl/what-is-https/)

🔗 [How HTTPS works? Comics](https://howhttps.works/)

---

## ⚖️ REST vs GraphQL

### REST (Representational State Transfer)

- Uses multiple endpoints for resources (e.g., `/users`, `/posts`).
- Follows HTTP conventions (GET, POST, PUT, DELETE).
- Simple and widely adopted.

### GraphQL

- Single endpoint (`/graphql`).
- Clients request exactly what they need (custom queries).
- Requires a schema and more tooling.

| Feature        | REST     | GraphQL                      |
| -------------- | -------- | ---------------------------- |
| Endpoints      | Multiple | Single                       |
| Overfetching   | Common   | Avoided                      |
| Learning Curve | Low      | Medium–High                  |
| Tooling        | Simple   | Needs tooling (Apollo, etc.) |

🔗 [GraphQL vs REST](https://aws.amazon.com/compare/the-difference-between-graphql-and-rest/)

---

## 🗂️ MIME Types

**MIME (Multipurpose Internet Mail Extensions) Types** tell the browser what type of content it is receiving.

Examples:

- `text/html` → HTML document
- `application/json` → JSON data
- `image/png` → PNG image
- `text/css` → Stylesheet

> The server includes MIME types in the `Content-Type` response header.

🔗 [MDN – Common MIME Types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types)

---

## 🧾 HTTP Methods & Status Codes

### Common HTTP Methods:

- `GET`: Retrieve data
- `POST`: Submit new data
- `PUT`: Update entire resource
- `PATCH`: Update part of a resource
- `DELETE`: Remove a resource

### Common Status Codes:

| Code | Meaning               |
| ---- | --------------------- |
| 200  | OK                    |
| 201  | Created               |
| 204  | No Content            |
| 301  | Moved Permanently     |
| 400  | Bad Request           |
| 401  | Unauthorized          |
| 403  | Forbidden             |
| 404  | Not Found             |
| 500  | Internal Server Error |

🔗 [MDN – HTTP Methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)

🔗 [MDN – Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

---

## 🔌 WebSockets (Brief Intro)

- Protocol for full-duplex communication between client and server.
- Unlike HTTP, it keeps the connection open.
- Ideal for real-time apps like chats, games, or live data feeds.

> Uses `ws://` or `wss://` instead of `http://`.

🔗 [MDN – WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)

🔗 [WebSockets Introduction – HTML5 Rocks (Archived)](https://www.html5rocks.com/en/tutorials/websockets/basics/)

---

## 📦 Caching & Headers

### Caching Basics

- **Browser Cache** stores previously fetched resources.
- Improves speed and reduces server load.

### Important Headers

- `Cache-Control`: How, when, and whether the response is cached.
- `ETag`: Helps identify resource changes.
- `Expires`: Sets a specific expiration date/time for content.
- `Last-Modified`: Timestamp of last change to the resource.

🔗 [MDN – HTTP Caching](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)

🔗 [Google Web Fundamentals – Caching](https://web.dev/http-cache/)

---

## ✅ Summary

Web protocols and networking concepts form the foundation of how clients communicate with servers. Understanding how HTTP, GraphQL, MIME types, methods, and caching work helps build more secure, performant, and maintainable web applications.

---
