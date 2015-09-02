name: inverse
layout: true
class: center, middle, inverse

---

# Osnove Web Tehnologija

.footnote[[Nemanja Nedeljković](https://nemanjan00.org/)]

---

## Kako sve to funkcioniše kao celina? 

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
]

.right-column[

  Browser: Hej, DNSu, gde se nalaze nameserveri za domenu peraperic.com? 

  DNS: Hej, oni su ns1.nesto.com i ns2.nesto.com

  Browser: Hej, ns1.nesto.com, koja je IP adresa za peraperic.com? 

  ns1.nesto.com: Hej, pa adresa je 192.168.1.244
]

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
  ## HTTP/S
]

.right-column[

  Browser: Hej, 192.168.1.244, daj mi taj i taj i taj fajl na domeni peraperic.com 

  192.168.1.244: Evo ti taj fajl

  

  HTTPS - Siguran HTTP [TLS - Transport Layer Security]
  
  POST, GET, PUT, DELETE
]

---

# Osnovni jezici na Webu [Frontend]

- HTML
- CSS
- JavaScript

---

# Magija na serveru [Backend] 

- HTTP Server
- Server-side scripting
- Baze podataka


- Production i development okruženja
- Virtualizacija i izolacija okruženja


- Održavanje servera
- Deployment

---

# Povećanje efikasnosti

- Organizacija razvojnog okruženja
- Frontend/Backend Framework
- Alati za povećanje efikasnosti
	- Virtualizacija razvojnog okruženja
	- Package managment
	- Automatizacija
