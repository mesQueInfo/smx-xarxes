# NetWorking Solutions — Fitxa de Treball (Sessió 15)

**Mòdul:** 0225 Xarxes Locals (CFGM SMX)
**Unitat Operativa:** NetWorking Solutions — BL2
**Títol:** Sistemes de Cablejat Estructurat (SCE) i Els seus subsistemes

**Alumnat / Equip:** ____________________________________  **Data:** ____________

---

## 1. Marc Teòric: Fonaments i Estructura del Cablejat Estructurat

Un Sistema de Cablejat Estructurat (SCE) és una infraestructura de xarxa de telecomunicacions dissenyada segons normes internacionals (ANSI/TIA-568, ISO/IEC 11801, EN 50173). Permet connectar equips informàtics, telèfons, servidors i dispositius actius d'una organització de manera integrada, flexible i fàcilment mantenible.

### Els 6 Subsistemes del Cablejat Estructurat

1. **Instal·lació d'Escomesa (Entrance Facility - EF):** Punt d'entrada dels serveis dels proveïdors de telecomunicacions (ISP, telefonia) a l'edifici. Hi trobem els dispositius de protecció i delimitació de responsabilitat.

2. **Sala d'Equipaments (Equipment Room - ER):** Espai centralitzat que allotja equips actius principals de gran capacitat (servidors principals, routers de sortida, PBX, commutadors principals). Acostuma a contenir el Distribuïdor de Campus (CD) o d'Edifici (BD).

3. **Subsistema de Cablejat Vertical / Troncal (Backbone):** Uneix els diferents distribuïdors de planta (FD) amb la Sala d'Equipaments (ER) o el Distribuïdor d'Edifici/Campus (BD/CD).
   - **Dades:** Es recomana l'ús de Fibra Òptica per suportar grans distàncies i altes velocitats sense interferències.
   - **Telefonia:** S'acostuma a utilitzar cable de parells de coure multiparell.

4. **Distribuïdor de Planta i Racks (Floor Distributor - FD / ER):** Armari o sala de comunicacions a cada planta on se situen els Patch Panels (taulers de connexions) i els Switches (commutadors actius) de la planta.

5. **Subsistema de Cablejat Horitzontal:** Comprèn tot el cablejat des del Distribuïdor de Planta (FD / Patch Panel) fins a les rosetes o preses de telecomunicacions d'usuari (TO).
   - **Mitjà habitual:** Cable de parells trenats (UTP / FTP / STP Cat 6 o superior).
   - **Distància màxima canal:** 100 metres en total (90 metres de cable permanent + màxim 10 metres totals en latiguillos/tirantets).

6. **Àrea de Treball (Work Area - WA):** Espai on s'ubiquen els usuaris finals. Comprèn des de la roseta o presa d'usuari (TO) fins als equips terminals (PC, impressora, telèfon IP) mitjançant latiguillos de xarxa.

### Interfícies i Rangs de Distància Recomanats

| Subsistema | Element d'Origen / Destí | Mitjà Recomanat | Límits de Distància / Observacions |
|---|---|---|---|
| Cablejat Horitzontal | Patch Panel (FD) a Presa Usuari (TO) | Cable UTP/FTP Cat 6 / 6A | Màxim 90 m d'enllaç permanent + 10 m de tirantets (Total 100 m) |
| Cablejat Vertical (Backbone) | FD (Planta) a BD/CD (Edifici/Campus) | Fibra Òptica (OM3/OM4 o OS2) | Fins a 300 m (Multimode) o km (Monomode) segons l'edifici |
| Àrea de Treball | Roseta (TO) a Equip Terminal | Latiguillo UTP Cat 6 | Longitud màxima recomanada de 3 a 5 metres |

---

## 2. Activitat Pràctica: Anàlisi i Auditoria d'un Sistema de Cablejat

### Part A: Identificació dels Subsistemes i Elements Tècnics

Respon les següents preguntes raonant la teva resposta a partir de la teoria anterior:

**1.** Un tècnic d'instal·lació ha de tirar un cable UTP Cat 6 des del Patch Panel de la planta 2 fins a una roseta situada a 96 metres de distància lineal. Complirà la normativa ANSI/TIA-568 / ISO 11801? Explica per què i quina solució tècnica caldria aplicar.

**Resposta:**

&nbsp;

**2.** Quin tipus de mitjà de transmissió és el més recomanat per al subsistema troncal o vertical d'un edifici d'oficines de 5 plantes on es requereix un alt ample de banda i immunitat al soroll electromagnètic? Justifica la tria.

**Resposta:**

&nbsp;

**3.** Relaciona mitjançant fletxes els següents conceptes de la columna A amb la seva definició o funció a la columna B:

| Columna A (Element / Abreviatura) | Columna B (Funció / Descripció) |
|---|---|
| 1. Presa de Telecomunicacions (TO) | A. Armari on es concentren els Patch Panels i equips actius de la planta. |
| 2. Floor Distributor (FD) | B. Punt de connexió final a l'àrea de treball on es connecta el PC (roseta). |
| 3. Cablejat Horitzontal | C. Enllaç entre la sala d'equips principal i els distribuïdors de planta. |
| 4. Cablejat Vertical (Backbone) | D. Tram de xarxa limitat a 90 m d'enllaç permanent més latiguillos. |

**Resposta:** 1 → ____ ; 2 → ____ ; 3 → ____ ; 4 → ____

---

### Part B: Disseny d'Infraestructura i Esquematització (Cas Pràctic)

**Escenari:** Una empresa ocupa un edifici de dues plantes (Planta Baixa i Planta 1). A la Planta Baixa hi ha la Sala d'Equipaments principal (ER) amb el servidor central i la connexió a Internet (EF). A la Planta 1 hi ha 20 llocs de treball que requereixen connexió a xarxa.

**Tasca de l'alumnat:**

1. Dibuixa un esquema de blocs simplificat on es mostrin els subsistemes de cablejat necessaris per connectar un ordinador de la Planta 1 amb el servidor situat a la Sala d'Equipaments (ER) de la Planta Baixa.

2. Completa la següent taula d'especificació de components per a la Planta 1:

| Component / Subsistema | Tipus d'Element o Cable proposat | Quantitat Estimada / Mètrica |
|---|---|---|
| Preses d'Usuari (TO) | Roseta Doble RJ-45 Cat 6 (Keystone) | 10 rosetes dobles (20 ports) |
| Cablejat Horitzontal | Cable UTP Cat 6 | Metres segons plànol (màx 90 m/cable) |
| Distribuïdor de Planta (FD) | Armari Rack 19" amb Patch Panel | 1 Rack de planta |
| Cablejat Vertical (Backbone) | Fibra Òptica Multimode o UTP Cat 6A | 1 tirada vertical (PB a P1) |

---

## 3. Check-List de Valoració de la Sessió

| Criteri d'Avaluació | Assolit (OK / KO) | Observacions |
|---|---|---|
| Identifica correctament els 6 subsistemes del cablejat estructurat | | |
| Aplica les normes de distància màxima en el cablejat horitzontal (100 m) | | |
| Tria el mitjà de transmissió adient per a cablejat vertical i horitzontal | | |
| Dissenya correctament un esquema funcional de xarxa per a un edifici | | |
