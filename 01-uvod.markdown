layout: true
class: center, middle, inverse

---

# Osnove Web Tehnologija

.footnote[[Nemanja Nedeljković](https://nemanjan00.org/)]

---

## Kako sve to funkcioniše kao celina?

---

layout: false

# Internet

.left-column[
  ## localhost
]

.right-column[
  ## Pojedinačni računar na mreži

  ### IP [192.168.1.x]

  ### Portovi

  80 - HTTP

  443 - HTTPS


  21 - FTP

  22 - SSH [FTPS]


]

---

# Internet

.left-column[
  ## localhost
  ## LAN
]

.right-column[
  ## Lokalna mreža

  ### Gateway [192.168.1.1]

  ### DHCP (Dodeljuje IP)
]

---

# Internet

.left-column[
  ## localhost
  ## LAN
  ## WAN
]

.right-column[
  ## Internet!

  ### Public IP

  ### NAT

  ### Port forwarding
]

---

layout: true
class: center, middle, inverse

---

## Ok, to su mreže, ali kako moj računar pronađe google.com?

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
]

.right-column[
  ## Protokol

  Browser: Hej, root DNSu, gde se nalazi TLD za domenu com?

  DNS Root: Na toj i toj adresi

  Browser: Hej TLD, gde se nalaze nameserveri za peraperic.com?

  TLD: Hej, oni su ns1.nesto.com i ns2.nesto.com

  Browser: Hej, ns1.nesto.com, koja je IP adresa za peraperic.com?

  ns1.nesto.com: Hej, pa adresa je 192.168.1.244

]

---

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
]

.right-column[
  ## Protokol

  <iframe width="560" height="315" src="https://www.youtube.com/embed/72snZctFFtA" frameborder="0" allowfullscreen></iframe>

]

---

layout: true
class: center, middle, inverse

---

## Ok, sada znam IP servera, ali kako računar dobija podatke sa tog servera?

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

layout: true
class: center, middle, inverse

---

## Dobro, sada imam fajlove, ali kako od gomile teksta i slika nastaje stranica?

---

layout: false

# Osnovni jezici na Webu [Frontend]

.left-column[

  ## HTML

]

.right-column[
  ## HTML [HyperText Markup Language]

  - HTML jezik koji opisuje sadržaj stranice.

  - Sačinjen je od blokova koda

  ```HTML
	<ime-taga atribut1="vrednost" atribut2=...> </imetaga>
  ```

  - Primer

  ```HTML
  <html>
	  <head>
		  <title>
			  Primer
		  </title>
	  </head>
	  <body>
		  <p>paragraf</p>
	  </body>
  </html>
  ```
]

---

layout: true
class: center, middle, inverse

---

## Ok, sadržaj je tu, ali ja hoću da ga ulepšam?

---

layout: false

# Osnovni jezici na Webu [Frontend]

.left-column[

  ## HTML
  ## CSS

]

.right-column[
  ## CSS [Cascading Style Sheets]

  - CSS je jezik koji opisuje izgled stranice [HTMLa]

  - Sačinjen je takođe od blokova koda

  ```CSS
  selector {property: value; property: value...}
  ```

  - Primer

  ```CSS
  body { /* Stil se odnosi na body blok */
	  color: white; /* Tekst je bele boje */
	  background-color: black; /* Boja pozadine je crna */
	  margin-top: 15px; /* Gornja margina je 15 pixela */
  }
  ```
]

---

layout: true
class: center, middle, inverse

---

## Još samo interaktivni deo! :)

---

layout: false

# Osnovni jezici na Webu [Frontend]

.left-column[

  ## HTML
  ## CSS
  ## JavaScript

]

.right-column[
  ## JavaScript

  - HTML je scripting jezik na frontendu

  - Nalazi se ili se referencira **&lt;script&gt;** tagom

  ```HTML
  <script src="https://code.jquery.com/jquery-2.1.4.min.js"></script>

  <script> /* neki kod */ </script>
  ```

  - Primer

  ```javascript
  var a = 5; var b = 3;

  if(a + b != 8){
		  document.write("JavaScript je idiot<br>");
  }

  alert("Neki tekst");
  ```
]


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

