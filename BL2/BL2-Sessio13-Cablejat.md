# Sessió 13: Cablejat de Xarxes Locals 

**Mòdul Professional:** 0225 - Xarxes Locals  
**Cicle Formatiu:** SMX (Sistemes Microinformàtics i Xarxes)  
**Bloc Temàtic:** Bloc 2

---

## 1. Introducció al Cablejat de Xarxes

En l'àmbit de les xarxes locals (LAN), la infraestructura de cablejat constitueix el medi físic encarregat de transportar les dades entre els diferents dispositius (ordinadors, servidors, commutadors, reencaminadors, etc.). Un disseny i una instal·lació adequats d'aquesta infraestructura són fonamentals per garantir la fiabilitat, velocitat i escalabilitat de la xarxa.

### 1.1 Tipus de medis de transmissió

1. **Cablejat de parell trencat (Twisted Pair):** El medi més comú en xarxes d'àrea local.
2. **Fibra òptica:** Utilitzada principalment per a grans distàncies o connexions d'alta velocitat (interconnexió d'edificis o *backbones*).
3. **Cable coaxial:** En desús per a xarxes d'àrea local modernes, mantenint-se en aplicacions específiques (TV per cable, connexions d'antena).

---

## 2. Cablejat de Parell Trencat

El cable de parell trencat consta de parells de fils de coure aïllats i trencats entre si per reduir les interferències electromagnètiques (EMI) i la diafonia (*crosstalk*).

### 2.1 Tipologies d'apantallament

* **UTP (Unshielded Twisted Pair):** Parell trencat sense apantallar. És el més econòmic i utilitzat en entorns d'oficina estàndard.
* **FTP / Foiled Twisted Pair (F/UTP):** Porta una pantalla d'alumini global que envolta tots els parells per protegir contra interferències exteriors.
* **STP (Shielded Twisted Pair):** Cada parell trencat disposa d'una malla de protecció individual.
* **SFTP / S/FTP (Screened Foiled Twisted Pair):** Disposa d'un apantallament individual per parell i una malla o pantalla global externa.

### 2.2 Categories de cables de coure

| Categoria | Amplada de banda | Velocitat màxima teòrica | Ús habitual |
| :--- | :--- | :--- | :--- |
| **Cat 5e** | 100 MHz | 1 Gbps (1000BASE-T) | Xarxes domèstiques / petites oficines |
| **Cat 6** | 250 MHz | 1 Gbps (10 Gbps a <55m) | Standard en instal·lacions comercials |
| **Cat 6a** | 500 MHz | 10 Gbps (10GBASE-T a 100m) | Xarxes corporatives i centres de dades |
| **Cat 7 / 7a**| 600–1000 MHz | 10 Gbps / 40 Gbps | Entorns industrials i alta densitat |
| **Cat 8** | 2000 MHz | 25 Gbps / 40 Gbps (a <30m) | Connexions de curt abast en Data Centers |

---

## 3. Estàndards de Connexió i Codis de Colors (RJ-45)

Els connectors **RJ-45** (8P8C) es crimpen seguint la norma **ANSI/TIA/EIA-568**. Existeixen dos estàndards de patró de colors:

### 3.1 Esquema T568A i T568B

| Pin | T568A (Color) | T568B (Color) |
| :---: | :--- | :--- |
| **1** | Blanc / Verd | Blanc / Taronja |
| **2** | Verd | Taronja |
| **3** | Blanc / Taronja | Blanc / Verd |
| **4** | Blau | Blau |
| **5** | Blanc / Blau | Blanc / Blau |
| **6** | Taronja | Verd |
| **7** | Blanc / Marró | Blanc / Marró |
| **8** | Marró | Marró |

### 3.2 Tipus de Cables segons la Configuració

* **Cable directe (*Straight-through*):** Utilitza la mateixa norma als dos extrems (T568B-T568B o T568A-T568A). s'utilitza per connectar dispositius de diferent tipus (ex: PC a Switch, Switch a Router).
* **Cable creuat (*Crossover*):** Utilitza T568A en un extrem i T568B en l'altre. S'utilitza tradicionalment per connectar dispositius del mateix tipus (ex: PC a PC, Switch a Switch).  
  *Nota: La majoria de dispositius moderns suporten **Auto-MDIX**, fent la detecció automàtica de creuament.*

---

## 4. Arquitectura de Cablejat Estructurat

Un sistema de cablejat estructurat (SCS) s'organitza de manera modular seguint la norma **TIA/EIA-568-C**.

```
[ Àrea de Treball ] 
       │ (Cable de connexió / Patch Cord)
       ▼
[ Roseta / Presa de Xarxa (TO) ]
       │ (Cablejat Horitzontal - Màx 90m)
       ▼
[ Armari de Comunicacions (TR/FD) ] ── (Patch Panels + Switches)
       │
       │ (Cablejat Vertical / Backbone)
       ▼
[ Armari Principal / Sala d'Equips (ER/CD) ]
```

### 4.1 Subsistemes del Cablejat Estructurat

1. **Àrea de Treball (WA - Work Area):** Comprèn des de les rosetes de connexió (RJ-45) fins als equips finals (PC, impressores, tèlèfons IP).
2. **Cablejat Horitzontal:** Enllaç que va des de les rosetes de l'àrea de treball fins a l'armari de distribució de planta (TR).  
   * **Distància màxima del canal:** 100 metres (90m de cablejat sòlid + 10m totals per a cables de connexió/patch cords).
3. **Armari de Distribució / Distribuidor de Planta (TR - Telecommunications Room / FD):** Allotja els patch panels, switches i elements de gestió.
4. **Cablejat Vertical o Backbone:** Interconnecta els diferents armaris de planta entre si i amb la sala d'equips principal. Normalment s'utilitza fibra òptica o cablejat de coure de gran capacitat.
5. **Sala d'Equips (ER - Equipment Room):** Espai centralitzat que allotja els servidors principals, routers de sortida a internet, PBX, etc.
6. **Entrada de Serveis (EF - Entrance Facilities):** PUNT on el proveïdor de serveis de telecomunicacions (ISP) introdueix les seves línies a l'edifici.

---

## 5. Mesures i Eines d'Instal·lació

Per a la realització d'una instal·lació professional de cablejat de xarxa es requereixen les següents eines i eines de verificació:

### 5.1 Eines de treball

* **Pelacables:** Eina per retirar la coberta exterior de protecció del cable sense danyar els parells interns.
* **Crimpadora RJ-45:** Eina de pressió mecànica per fixar els pins del connector RJ-45 sobre els conductors de coure.
* **Eina d'impacte (Punch-down tool):** S'utilitza per inserir i tallar els cables en els mòduls femella (Keystone) i en els *patch panels* (connectors tipus IDC/110).

### 5.2 Verificació i Certificació

* **Tester continuïtat / Provador de cableat:** Comprova si tots els pins estan ben interconnectats, si hi ha curtcircuits o parells oberts.
* **Certificador de xarxa:** Equip d'alta precisió que mesura paràmetres crítics com l'atenuació, la diafonia (NEXT, FEXT), la pèrdua de retorn i la longitud. És imprescindible per garantir que la instal·lació compleix la categoria especificada.

---