## What is a Service Worker?

A **service worker** is a special JavaScript file that:

* Runs in the background
* Is **separate from your web page**
* Intercepts network requests
* Has **no direct access to the DOM**
* Works even when the page is closed (in some cases)

It sits **between your app and the network**.

```
Browser
   ↓
Service Worker  ← interception happens here
   ↓
Network / Cache
```

Service workers let you:

* Cache intelligently
* Control offline behavior
* Improve performance
* Enable native-like features

Example:

```js
self.addEventListener("fetch", event => {
  event.respondWith(
    caches.match(event.request).then(res => {
      return res || fetch(event.request)
    })
  )
})
```

---

## How to Use a Service Worker

### 1. Register it (Frontend)

```js
if ("serviceWorker" in navigator) {
  navigator.serviceWorker.register("/sw.js")
}
```

---

### 2. Create `sw.js`

```js
self.addEventListener("install", event => {
  event.waitUntil(
    caches.open("v1").then(cache =>
      cache.addAll(["/", "/index.html"])
    )
  )
})
```

---

### 3. Control Fetch

```js
self.addEventListener("fetch", event => {
  event.respondWith(fetch(event.request))
})
```
