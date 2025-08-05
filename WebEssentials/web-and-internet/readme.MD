# 🌐 The Web and Internet Basics

This section covers the foundational concepts behind how the web and internet function. Understanding these basics is essential before diving into frontend or backend development.

---

## 📌 Topics Covered

- What is the Web?
- Internet vs. Web
- How the Internet Works
- Client-Server Model
- Request & Response Cycle
- URL Structure & Query Parameters
- Domain Names & DNS
- IP Address & Hosting

---

## 🌍 What is the Web?

The **World Wide Web (WWW)** is a collection of interlinked documents and applications accessed via the internet using web browsers.

- Built on top of the **internet**
- Uses **HTTP/HTTPS** protocols
- Accessed through **browsers**

🔗 [MDN – How the Web works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

---

## 🌐 Internet vs Web

| Feature    | Internet                   | World Wide Web               |
| ---------- | -------------------------- | ---------------------------- |
| Definition | Global network of networks | Collection of documents/apps |
| Protocols  | TCP/IP, UDP                | HTTP, HTTPS                  |
| Access     | Routers, ISPs              | Browsers                     |
| Services   | Email, FTP, VoIP, Web      | Web pages, Web apps          |

🔗 [Internet vs WWW](https://www.scaler.com/topics/difference-between-internet-and-www/)

---

## 🖧 How the Internet Works (Simplified)

1. You type a URL into the browser.
2. Browser performs **DNS lookup** to find IP address.
3. Sends **HTTP request** to the server.
4. Server returns **HTML, CSS, JS**.
5. Browser renders the page.

🔗 [MDN – How does the Internet work?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work)

## 🔗 [How HTTPS works? Comics](https://howhttps.works/)

## 🧑‍💻 Client-Server Model

- **Client**: The browser or device making the request
- **Server**: The machine hosting the web content
- Communication happens over **HTTP** or **HTTPS**

> Client requests → Server responds

🔗 [Understanding Client–Server Model](https://systemdesignschool.io/blog/client-server)

---

## 🔁 Request & Response Cycle

- **Request**:

  - Method: GET, POST, etc.
  - Headers
  - Body (for POST/PUT)

- **Response**:

  - Status Code (200, 404, etc.)
  - Headers
  - Body (HTML, JSON, etc.)

🔗 [MDN – HTTP Request and Response](https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages)

---

## 🔗 URL Structure & Query Parameters

A URL (Uniform Resource Locator) looks like:

```
https://www.example.com/path?query=value
```

- **Scheme**: `https`
- **Host**: `www.example.com`
- **Path**: `/path`
- **Query**: `?query=value`

🔗 [MDN – URL Basics](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_URL)

---

## 🧭 Domain Names & DNS

- **Domain Name**: Human-friendly name (e.g., `google.com`)
- **DNS**: Translates domain to IP address
- Like a phonebook for the internet

🔗 [Cloudflare – What is DNS?](https://www.cloudflare.com/learning/dns/what-is-dns/)

🔗 [How DNS works? Comics](https://howdns.works/)

---

## 🖥️ IP Address & Hosting

- **IP Address**: Unique address for each device/server on the internet
- **Hosting**: A service that stores your website files and serves them to users

🔗 [Namecheap – What is Web Hosting?](https://www.namecheap.com/guru-guides/what-is-web-hosting/)

---

## ✅ Summary

Understanding how the web and internet function together sets the foundation for everything in web development. Concepts like DNS, URLs, HTTP, and client-server architecture are essential to building, debugging, and deploying modern web applications.

---
