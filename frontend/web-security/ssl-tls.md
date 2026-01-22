## 1️⃣ What SSL/TLS Is

* **SSL** = Secure Sockets Layer (old)
* **TLS** = Transport Layer Security (modern, secure version)
* They **encrypt data between client and server**, so no one can read it on the network.

---

## 2️⃣ Why We Use It

* Encrypt sensitive info (passwords, wallet data, APIs)
* Ensure **data integrity** (no tampering)
* Confirm server identity (**HTTPS padlock**)

---

## 3️⃣ How It Works

1. **Handshake**

   * Browser asks server: “Let’s talk securely”
   * Server sends its **TLS certificate** (public key, signed by CA)
   * Browser checks certificate validity (signed, not expired, matches domain)

2. **Key Exchange**

   * Browser and server agree on a **session key** (symmetric key)
   * This key encrypts all data for the session

3. **Secure Communication**

   * All HTTP requests/responses are now encrypted (`HTTPS`)

## References
- https://www.youtube.com/watch?v=0yw-z6f7Mb4
- https://www.youtube.com/watch?v=THxIyHz191A
