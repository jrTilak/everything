# How Does the Internet Work?

The **internet** is the backbone of the modern web. It is the global technical infrastructure that allows computers and devices around the world to communicate with each other. At its core, the internet is a massive **network of networks**, connected through wired (fiber, copper) and wireless (Wi-Fi, cellular, satellite) links.

## Servers and Clients

A **server** is a special computer that is directly connected to the internet and is always ready to respond to requests. Every server has a unique **IP address** (Internet Protocol address), which acts like a phone number for computers.

Because IP addresses are hard for humans to remember, we use **domain names** (like `example.com`). These names are simply human-friendly labels that point to IP addresses.

Your personal computer or phone is usually **not a server**. Instead, it acts as a **client** and connects to the internet through an **ISP (Internet Service Provider)**, such as a broadband or mobile network.

## DNS: From Domain Name to IP Address

When you type a domain name into your browser:

1. Your computer asks a **DNS (Domain Name System)** server for the IP address of that domain.
2. The DNS server responds with the correct IP address.
3. Your computer now knows where to send the request.

DNS is often compared to a global phone book for the internet.

## Data Transfer and Packets

Once the connection is established:

- The **client** (your computer) and the **server** exchange data.
- This data is broken into small pieces called **packets**.
- Each packet contains:
  - The source IP address
  - The destination IP address
  - A small chunk of the actual data

Packets can travel through different paths across the internet, depending on traffic and network conditions.

When all packets reach their destination, they are **reassembled** in the correct order to recreate the original information, such as a web page, image, or video.

## Routers: Guiding the Packets

So how do packets know where to go?

This is the job of **routers**.

- Routers are networking devices that sit between networks.
- They examine the destination IP address of each packet.
- Based on routing tables, they forward the packet to the next best route toward its destination.

Think of routers as traffic controllers, constantly choosing efficient paths so data can flow smoothly across the internet.

## Protocols: The Rules of Communication

The internet works because everyone follows the same rules, called **protocols**, such as:

- IP (Internet Protocol)
- **TCP (Transmission Control Protocol)**
- **HTTP/HTTPS**

Without these shared rules, computers would speak different languages and communication would fall apart.

## Summary

In simple terms:

- The internet connects computers worldwide.
- Domain names are translated into IP addresses using DNS.
- Data is sent as packets through routers.
- Packets are reassembled at the destination.
- Standard protocols make communication reliable.

## References

- [How the Internet Works in 5 Minutes](https://www.youtube.com/watch?v=7_LPdttKXPc)
- [How Does the Internet Work? – MDN Docs](https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work)
