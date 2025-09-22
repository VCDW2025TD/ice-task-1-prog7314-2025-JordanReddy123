
1. What is SSL/TLS, and how do they differ?

* **SSL (Secure Sockets Layer)** and **TLS (Transport Layer Security)** are cryptographic protocols that secure communication over the internet.
* They work by encrypting data exchanged between a client (e.g., browser) and a server so that attackers can’t read or modify it in transit.

Key difference:

* SSL is the older protocol.
* TLS is its successor — it’s more secure and efficient.
* In practice, when people say “SSL certificate,” they usually mean **TLS certificate**, since SSL is largely deprecated.

---

2. Why is HTTPS more secure than HTTP?

HTTP sends data **in plain text**, meaning anyone intercepting the network traffic (like on public Wi-Fi) can read it.
HTTPS, which is HTTP running over SSL/TLS, provides:

✅ **Encryption** – protects data (e.g., passwords, credit card numbers).
✅ **Authentication** – ensures you’re communicating with the legitimate website.
✅ **Data Integrity** – prevents attackers from modifying content (e.g., injecting malicious scripts).

Example:

* HTTP request: `username=alice&password=12345` → easily readable by an attacker.
* HTTPS request: Encrypted payload → attacker only sees gibberish.

---

3. Risks of not using SSL in web applications

If you don’t use SSL/TLS, you risk:

 **Data theft:** Attackers can sniff sensitive data like passwords or payment info.
 **Man-in-the-Middle (MITM) attacks:** Hackers can intercept and modify data in transit.
 **Phishing / Impersonation:** Without authentication, users can’t be sure they’re on the real site.
**SEO penalties:** Search engines (like Google) penalize sites without HTTPS.
 **Browser warnings:** Modern browsers show a “Not Secure” warning for HTTP sites, scaring users away.

---

4. Real-World Incidents Involving Missing or Misconfigured SSL


* **Equifax (2017)** – One contributing factor in their massive data breach was an unencrypted internal system that exposed sensitive data during transmission.
* **Panama Papers (2016)** – The law firm Mossack Fonseca had client login portals with outdated SSL/TLS configurations, making them easier to exploit.
* **Tesco Bank (2016)** – Poor SSL implementation and weak cryptography contributed to attackers being able to carry out fraud.
* **Cloudflare “Cloudbleed” (2017)** – A misconfiguration caused data leaks over HTTPS, proving that even when SSL is used, poor implementation can still create vulnerabilities.

---
