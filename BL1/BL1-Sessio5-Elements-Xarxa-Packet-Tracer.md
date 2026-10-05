# SESSIÓ 5: ELEMENTS DE XARXA I INTEGRACIÓ AMB PACKET TRACER

**Mòdul:** SMX MP05 - Xarxes Locals  
**Nom de l'alumne/a:** ___________________________________  
**Data:** ____________________

---

## OBJECTIUS DE LA SESSIÓ

1. Analitzar el comportament del domini de col·lisió i difusió utilitzant diferents dispositius de xarxa (Hub, Switch, Repetidor, Access Point, Router i Bridge).
2. Configurar direccions IP i provar el trànsit en mode simulació (Packet Tracer).
3. Dissenyar i interconnectar la xarxa local d'un centre educatiu complint restriccions d'equipament i rendiment.

---

## PART 1: COMPORTAMENT DELS DISPOSITIUS DE XARXA

Dibuixa i simula cada una de les següents topologies amb el programa Cisco Packet Tracer. Respon a les preguntes utilitzant el mode simulació (Simulation Mode) per veure el recorregut dels paquets. Desa cada simulació com un fitxer separat.

---

### 1. HUB

- **Disseny:** Connecta 4 ordinadors (PC0, PC1, PC2, PC3) i 1 servidor (Server1) a un Hub.
- **Configuració:** Fes servir l'adreçament IP 192.168.1.X /24.

![Diagrama Hub](imatges/01_hub.png)

**Preguntes:**

1. Envia un paquet del PC2 al PC3. Explica què passa a la xarxa quan el paquet arriba al Hub.
2. Envia un paquet simultàniament del PC0 al Server1 i del Server1 al PC0. Què passa i per què?

---

### 2. SWITCH

- **Disseny:** Connecta 4 ordinadors (PC0, PC1, PC2, PC3) i 1 servidor (Server1) a un Switch.
- **Configuració:** Fes servir l'adreçament IP 192.168.1.X /24.

![Diagrama Switch](imatges/02_switch.png)

**Preguntes:**

1. Envia un paquet del PC2 al PC3. Explica què passa a la xarxa.
2. Envia un paquet simultàniament del PC0 al Server1 i del Server1 al PC0. Què passa i quina diferència hi ha respecte al Hub?

---

### 3. REPETIDOR

- **Disseny:** Connecta 3 ordinadors (PC0, PC4, PC5) a un Hub (Hub0). Connecta aquest Hub mitjançant un cable creuat a un Repetidor (Repeater3) i, a l'altre extrem, connecta un ordinador (PC1).
- **Configuració IP:** Totes les adreces IP han de començar per 192.168.1.X.

![Diagrama Repetidor](imatges/03_repetidor.png)

**Preguntes:**

1. Envia un paquet del PC4 al PC5. El PC1 rep algun paquet? Per què?
2. A quin altre dispositiu de xarxa s'assembla el repetidor pel que fa al seu funcionament a nivell de difusió?

---

### 4. PUNT D'ACCÉS (ACCESS POINT)

- **Disseny:** Connecta 3 PC per cable (PC0, PC1, PC2) a un Switch (Switch0). Connecta el Switch a un Access Point (AccessPoint0) i afegeix 4 ordinadors sense fils (PC3, PC4, PC5, PC6).
- **Configuració IP:** Totes les adreces IP han de començar per 10.0.0.X /8.

![Diagrama Access Point](imatges/04_access_point.png)

**Preguntes:**

1. Fes les proves necessàries per respondre: A quin altre dispositiu de xarxa s'assembla el punt d'accés pel que fa al seu funcionament de difusió del senyal? Per què?

---

### 5. ROUTER

- **Disseny:** Connecta 5 ordinadors (PC0, PC1, PC2, PC7, PC9) a un Switch (Switch0) i el Switch a una interfície FastEthernet d'un Router (Router0).
- **Configuració:** Configura la IP del Router com a Gateway predeterminada de tots els ordinadors.

![Diagrama Router](imatges/05_router.png)

**Preguntes:**

1. El router es comporta com un ordinador més de la xarxa o té una funció diferent? *(Respon les preguntes d'aquesta secció en color blau).*

---

### 6. BRIDGE (PONT)

- **Disseny:** Connecta 3 ordinadors (PC3, PC6, PC7) a un Hub (Hub2). Connecta el Hub a un Bridge (Bridge0) i l'altre extrem del Bridge a un ordinador (PC2).
- **Configuració IP:** Totes les adreces IP han de començar per 10.0.0.X /8.

![Diagrama Bridge](imatges/06_bridge.png)

**Preguntes:**

1. Envia un paquet del PC6 al PC7. El PC2 rep algun paquet? Per què?
2. A quin altre dispositiu de xarxa s'assembla el Bridge pel que fa al seu funcionament?

---

## PART 2: DISSENY D'UNA XARXA LOCAL PER A UN INSTITUT

Dissenya una xarxa d'àrea local (LAN) i comprova el seu funcionament mitjançant el programa Packet Tracer.

### Escenari

S'ha d'instal·lar una xarxa en una planta d'un institut que disposa de quatre aules:

- Aula 1
- Aula 2
- Aula 3
- Aula 4

### Requisits i Condicions

1. **Ordinadors per aula:** Hi ha 12 ordinadors per cada aula.
2. **Nomenclatura dels equips:** Els equips de cada aula s'anomenaran seguint el patró `A<N>-PC<M>` (per exemple: A1-PC1, A1-PC2, ..., A4-PC12).
3. **Adreçament IP:** Totes les IP han de començar per 192.168.1.X amb la màscara 255.255.255.0.
4. **Inventari de dispositius disponible (LÍMIT ESTRICTE):**
   - Només disposeu de **5 HUBS** i **3 SWITCHS** de 10 ports cadascun.
   - Cal anomenar aquests dispositius indicant l'aula on es troben (Exemple: hub1_aula1, hub2_aula1, switch1_aula1).
5. **Aïllament del trànsit i Rendiment (MOLT IMPORTANT):**
   - El rendiment de cada aula no s'ha de veure afectat pel trànsit intern de les altres aules.
   - Heu de comprovar i demostrar que quan s'envia un paquet entre dos ordinadors de la mateixa aula, aquest paquet no arriba mai als ordinadors de les altres aules.

---

## PART 3: SIMULACIÓ DE L'AULA REAL

1. Dibuixa i simula l'aula de classe en la qual et trobes actualment.
2. Inclou almenys un ordinador portàtil que es connecti per Wi-Fi.
3. Suposa que la connexió a Internet prové d'un Home Router (Switch/Router Wi-Fi).
4. Utilitza un Switch de 24 ports per interconnectar els equips cablats.

---

**Lliurament:** Lliura els fitxers de simulació `.pkt` generats juntament amb les respostes d'aquesta guia.
