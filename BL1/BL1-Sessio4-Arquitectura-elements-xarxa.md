# TEORIA [BL1. El Camp d'entrenament](BL1-Camp-Entrenament.md)

# SESSIÓ 4

**Títol:** Diagnòstic d'Incidències per Capes i Procés d'Encapsulació, Desencapsulació i Estructura de les PDU
**Durada:** 2 hores


## 1. Marc teòric de consulta ràpida

| Capa OSI | Nom capa OSI | Equiv. TCP/IP | PDU | Direccionament / capçalera clau |
|---|---|---|---|---|
| 7 | Aplicació | Aplicació | **Dades** | Protocol d'aplicació (HTTP, SSH, DNS...) |
| 6 | Presentació | Aplicació | **Dades** | Format i xifrat (SSL/TLS, ASCII...) |
| 5 | Sessió | Aplicació | **Dades** | Gestió de diàleg i connexió (RPC, SQL) |
| 4 | Transport | Transport | **Segment** (TCP) **Datagrama** (UDP) | Ports origen i destinació (TCP / UDP) |
| 3 | Xarxa | Internet | **Paquet** | Adreces IP origen i destinació |
| 2 | Enllaç de dades | Accés a la xarxa | **Trama** | Adreces MAC origen i destinació |
| 1 | Física | Accés a la xarxa | **Bits** | Senyals elèctrics, òptics o ones |

---

# 🛠️ FITXA DE TREBALL
**Unitat Operativa:** NetWorking Solutions | **Mòdul:** 0225  
**Alumnat / Equip:** ____________________________________ **Data:** ____________

---

## 📋 TALLER 1: MATERIAL DE L'ALUMNAT — Full d'Incidències de Client


> **Instruccions:** analitza els problemes reportats. Determina la capa OSI afectada (capa 1 a capa 7), la PDU corresponent i redacta la justificació tècnica.
>
### Objectius

> - Anàlisi comparativa: les 7 capes del model teòric OSI respecte a les 4 capes pràctiques del model TCP/IP.
- Control de diàleg i flux: funcions de sincronització, estructuració, control d'errors i recuperació de sessions.
- Relació maquinari–capa: NIC, Hub i Repetidor (capa 1); Switch, Bridge i Access Point (capa 2); Router (capa 3).


### Incidència 01

> Un usuari no pot accedir a la intranet mitjançant `https://intranet.empresa.local`. Tanmateix, la connexió física és correcta i el comandament `ping` a la IP del servidor respon sense pèrdues de paquets.

| Camp | Resposta |
|---|---|
| **Capa OSI afectada** | |
| **PDU associada** | |
| **Justificació tècnica** | |


### Incidència 02

> L'indicador lluminós del port RJ-45 de la targeta NIC està apagat. El sistema operatiu mostra el missatge "Cable de xarxa desconnectat".

| Camp | Resposta |
|---|---|
| **Capa OSI afectada** | |
| **PDU associada** | |
| **Justificació tècnica** | |


### Incidència 03

> Un equip no pot comunicar-se amb les màquines d'una altra subxarxa llunyana. El diagnòstic mostra que la màscara de xarxa o la porta d'enllaç per defecte (IP del router) estan mal configurades.

| Camp | Resposta |
|---|---|
| **Capa OSI afectada** | |
| **PDU associada** | |
| **Justificació tècnica** | |


### Incidència 04

> Un switch de la capa d'accés ha omplert la seva taula d'adreces MAC a causa d'un atac i ha començat a retransmetre el tràfic per tots els seus ports.

| Camp | Resposta |
|---|---|
| **Capa OSI afectada** | |
| **PDU associada** | |
| **Justificació tècnica** | |


---

# 🛠️ FITXA DE TREBALL
**Unitat Operativa:** NetWorking Solutions | **Mòdul:** 0225  
**Alumnat / Equip:** ____________________________________ **Data:** ____________

---

## 📋 TALLER 2: MATERIAL DE L'ALUMNAT Taller d'Encapsulació i PDU

## 1. Objectius didàctics

- Dominar el procés d'afegir i extreure capçaleres (encapsulació / desencapsulació).
- Descompondre les estructures de les unitats de dades de protocol (PDU): Dades, Segment, Paquet, Trama i Bits.
- Identificar l'adreçament físic (MAC) i lògic (IP) present a les capçaleres.

## EXPLICACIÓ

- L'encapsulació de dades: com les dades de l'aplicació van descendint per la pila afegint la capçalera de transport (ports TCP/UDP), la capçalera de xarxa (IPs), la capçalera d'enllaç (MACs + FCS), fins a convertir-se en bits sobre el medi físic.
- Desencapsulació: procés invers que realitza el host receptor o el dispositiu intermediari (un router desencapsula fins a capa 3 per llegir la IP; un switch ho fa fins a capa 2 per llegir la MAC).

### Part 1: Sectors de la PDU en trànsit

*Analitza el flux de transmissió següent i omple els camps de les capçaleres amb la informació proporcionada:*

| Dades enviades: "GET /index.html HTTP/1.1" | |
|---|---|
| **Port origen:** 51234 | **Port destinació:** 80 (HTTP) |
| **IP origen:** 192.168.1.25 | **IP destinació:** 193.147.87.40 |
| **MAC origen:** 00:1A:2B:3C:4D:5E | **MAC destinació:** 00:11:22:AA:BB:CC |

#### 1. Capa d'enllaç (Trama)

| Camp | Resposta |
|---|---|
| PDU | |
| MAC origen | |
| MAC destinació | |

#### 2. Capa de xarxa (Paquet)

| Camp | Resposta |
|---|---|
| PDU | |
| IP origen | |
| IP destinació | |

#### 3. Capa de transport (Segment)

| Camp | Resposta |
|---|---|
| PDU | |
| Port origen | |
| Port destinació | |

#### 4. Capa d'aplicació

| Camp | Resposta |
|---|---|
| PDU | |
| Dades | |

### Part 2: Qüestionari tècnic de validació

**1. Quin dispositiu de xarxa analitza la capçalera de la Trama (capa 2) per prendre decisions de reenviament?**

☐ Router &nbsp;&nbsp;&nbsp;&nbsp; ☐ Switch &nbsp;&nbsp;&nbsp;&nbsp; ☐ Repetidor

**2. Quin dispositiu de xarxa desencapsula la trama fins a arribar a la capçalera del Paquet (capa 3) per decidir la millor ruta?**

☐ Hub &nbsp;&nbsp;&nbsp;&nbsp; ☐ Switch capa 2 &nbsp;&nbsp;&nbsp;&nbsp; ☐ Router

**3. Quan el paquet surt de la xarxa local cap a Internet a través del router, quines adreces canvien a la trama de capa 2?**

```
