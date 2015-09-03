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

  Browser: Hej, root DNSu, gde se nalazi TLD za domenu com? 

  DNS Root: Na toj i toj adresi

  Browser: Hej TLD, gde se nalaze nameserveri za peraperic.com? 

  TLD: Hej, oni su ns1.nesto.com i ns2.nesto.com

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
  ## Protokol

  Browser: Hej, 192.168.1.244, daj mi taj i taj fajl na domeni peraperic.com, a evo ti i neki argumenti 

  192.168.1.244: Evo ti taj fajl
]

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
  ## HTTP/S
]

.right-column[

  ## Osnovni zahtevi

  POST - Slanje nekih podataka npr. iz forme [Prosleđuje argumente u samom zahtevu]

  GET - Zahtev za podacima [može da prosledi neke argumente u URLu]

  HEAD - Isto kao i GET, samo što se vraća samo HEADER odgovora

  ## Ređe korišćeni zahtevi

  PUT - Sačuvaj podatke na toj adresi

  DELETE - Obriši podatke sa te adrese
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
