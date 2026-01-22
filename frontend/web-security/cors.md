## **CORS (Cross-Origin Resource Sharing):**

A **browser security rule** that controls which websites can call your backend APIs.

### How it works

Browser sends a request with:

```
Origin: https://frontend.com
```

Backend replies with:

```
Access-Control-Allow-Origin: https://frontend.com
```

If they don’t match → browser blocks the response.

---

### Preflight

For non-simple requests (POST with JSON, headers, auth):

* Browser sends **OPTIONS** request first
* Server must allow it

### When to care

* Frontend and backend on **different domains/ports**
* Using **cookies, auth headers, or POST/PUT/DELETE**


