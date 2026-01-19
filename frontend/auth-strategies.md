# Authentication Strategies

## Basic Authentication

```http
Authorization: Basic <base64-encoded-username:password>
```

- Username and password are sent with every request
- Base64 is only encoding, not encryption
- Not considered secure
- Should only be used over HTTPS

---

## Session-Based Authentication

- User is assigned a **unique identifier (session ID)**
- Session ID is stored on the server (memory or database)
- Client sends the session ID with every request
- Server uses the session ID to verify the user

```http
# Header
X-Session-Id: ...
# or via cookies
Cookie: session_id=...
```

- **Stateful authentication**
- Easy to revoke session

---

## Token-Based Authentication

- Client sends credentials to generate a token
- Server generates a token and sends it to the client
- Server may optionally store tokens for early invalidation
- Token can be decoded to get user data
- Token usually has an expiry time

### Characteristics of tokens

- Random string or structured token
- Usually **stateless** (server does not store state)
- Has an expiry date
- Sent in the `Authorization` header
- Signed using a secret

Examples: JWT, SWT

---

## JWT-Based Authentication

JWT (JSON Web Token) is a type of token-based authentication.

```http
Authorization: Bearer <jwt-token>
```

**Format**

```
header.payload.signature
```

---

## OAuth

OAuth is an **authorization protocol** that allows users to share limited access to their private resources with third-party applications.

Example: Login with Google, GitHub access for third-party apps

---

## SSO (Single Sign-On)

SSO is an authentication strategy that allows users to log in once and access multiple related but independent services.

Example:
A single Google account can be used to access Gmail, YouTube, Google Calendar, and Docs

## References

- [Basic Authentication](https://roadmap.sh/guides/basic-authentication)
- [Session Based Authentication](https://roadmap.sh/guides/session-based-authentication-visually-explained)
- [Token Based Authentication](https://roadmap.sh/guides/token-authentication)
- [JWT Authentication](https://roadmap.sh/guides/jwt-authentication)
- [OAuth](https://roadmap.sh/guides/oauth)
- [SSO](https://roadmap.sh/guides/sso)
