---
marp: true
# theme: undercover

theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.jpg')

---
<style>
strong {
  color: #f44336 !important;
}
</style>
![bg right:40% 80%](img/logo2.png)

# Nätverksutrustning
## Digital kommunikationsteknik

---

# Mål!
## Översikt av olika typer av nätverksutrustning
Använd de röda markeringarna för att göra anteckningar….

---

![bg left:40% 80%](img/hub.png)

# HUB
 - Ansluter enheter till nätverket 
 - All data som hubben tar emot skickas ut till alla portar på hubben (förstärkt)
 - Enkel utrustning som är föråldrad idag och används inte mer. 
 - Dålig prestanda
 - Dålig säkerhet
 - Jobbar enbart på fysisk nivå(Läser ej frames)

---

<style scoped>
    section {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>

![width:100% height:100%](img/hub_how.gif)

---

<style scoped>
    ul {
        font-size: 24px;
    }
</style>

![bg right:40% 80%](img/switch.png)

# SWITCH
 - Ansluter enheter till nätverket 
 - En switch jobbar på lager 2 i OSI-modellen
 - En switch läser av alla ”frames” och noterar avsändare och håller koll på mottagare **(för adressering används MAC-adresser)**
 - Detta görs med en MAC-table
 - En switch skickar bara frames till den port som switchen vet att mottagaren är ansluten till
 - Är mottagaren av en frame okänd så skickas frame’en ut på alla portar (utom sändarens). Kallas flooding. 
 - En switch lär sig **MAC-adresser** genom att läsa av användar-**MAC-adressen** på inkommande frames. 
 - Betydligt **bättre säkerhet och prestanda än en HUB**

---

<style scoped>
    section {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>

![width:100% height:100%](img/switch_how.gif)

---

<style scoped>
    ul {
        font-size: 24px;
    }
</style>

![bg right:40% 80%](img/router.png)

# ROUTER
 - Används till att koppla samman nätverk med varandra
 - En router jobbar minst på nivå 3 enligt OSI-modellen (Paketnivå (**IP**) och uppåt)
 - Routrar är avancerade nätverksenheter som uppför sig som datorer och kör någon form av OS
 - Routrar är komplexa och flexibla och kan har flera **roller i nätverket** T.ex. agera brandvägg och/eller övervaka nätverkstrafiken
 - Använder en routing table för att skicka paketen rätt. 

---

![bg right:40% 80%](img/hemmarouter.png)

# HEMMAROUTER
 - ISR (Integrated Service Router) även kallad en **multi-function device** eller hemmarouter/bredbandsrouter. 
 - Allt-i-ett enhet som fungerar som en **switch, router, accesspunkt, (modem). Oftast med brandväggsfunktioner.**
 - Billiga 
 - Fungerar bra till mindre nätverk

---

![bg left:40% 80%](img/repeater.png)


# REPEATER
 - Upprepar signalen
 - Tar emot signalen och förstärker den för att sedan skicka vidare signalen
 - Används för att utöka räckvidden
 - Alla hubbar och switchar förstärker även signalen

---

<style scoped>
    section {
        display: grid;
        grid: auto / 2fr 1fr;
    }
    h1 {
        grid-column: 1 / 2;
    }
    ul {
        grid-column: 1 / 2;
    }
    img {
        grid-column: 2 / 3;
    }
</style>

# MODEM
 - Modulator-Demodulator
 - Omvandlar digitala signaler till analoga och tvärt om
 - Används för att skicka data över ett analogt mediumT.ex. telefonlinjen !
 - Modem används främst till: 
    Traditionell telefonlinje 
    DSL
    Kabel

![width:300px height:100%](img/modem1.png)
![width:300px height:100%](img/modem2.png)
[Lyssna på modemet!](https://www.youtube.com/watch?v=aV8DEJ8ydJQ)

---

<style scoped>
    section {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>

![bg center:90% 90%](img/dsl.png)

---
<style scoped>
    section {
        display:grid;
        grid: 1fr 1fr / 2fr 1fr;
    }
    ul {
        list-style: none;
        padding: 0;
    }
</style>

- # NÄTVERKSKORT
- ### **NIC** - **N**ETWORK **I**NTERFACE **C**ARD

* ![width:300px height:100%](img/nic1.png)
* ![width:300px height:100%](img/nic2.png)

---

# ACCESSPUNKT
 - **Wireless Access Point (AP)**
 - Kopplar samman flera trådlösa enheter med varandra och (oftast) ett trådbundet nät
 - **Kan ses som en HUB/Switch för trådlösa enheter**
 - Det finns flera olika standarderför WLAN och därmed flera varianter på AP

---
<style scoped>
    section {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }
    img {
        width: 200%;
    }
</style>

![Tux, the Linux mascot](img/ap1.png)

![Tux, the Linux mascot](img/ap2.png)

![Tux, the Linux mascot](img/ap3.png)

---

<style scoped>
    section {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>

![bg center:60% 60%](img/avslut.png)

<!-- ![Tux, the Linux mascot](test.png)

[Read more about MD](https://https://www.markdownguide.org/basic-syntax/). -->

---