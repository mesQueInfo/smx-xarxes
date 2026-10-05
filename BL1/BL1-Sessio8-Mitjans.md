## Apartat 1: Classificació i Selecció de Mitjans de Transmissió

### Exercici 1: Taula comparativa de mitjans

Classifica cadascun dels següents mitjans de transmissió omplint les dades corresponents a la taula:

* Cable de parell trencat no blindat (UTP)
* Fibra òptica monomode
* Ona de ràdio per radiodifusió
* Cable coaxial
* Enllaç sense fils Wi-Fi (WLAN)

| Mitjà de transmissió | Tipus de mitjà (Guiat / No guiat) | Senyal físic (Elèctric / Òptic / Electromagnètic) | Tipus de senyal (Analògic / Digital) |
| --- | --- | --- | --- |
| **Cable UTP** |  |  |  |
| **Fibra òptica monomode** |  |  |  |
| **Ona de ràdio FM** |  |  |  |
| **Cable coaxial** |  |  |  |
| **Enllaç Wi-Fi** |  |  |  |

---

### Exercici 2: Selecció de mitjans per a casos pràctics

Tria el mitjà de transmissió més adequat per a cadascun dels següents escenaris i justifica breument la teva opció:

* **Cas A:** Interconnectar dos edificis d'una fàbrica separats per $1,5\text{ km}$ en un entorn amb molta maquinària que genera fort soroll electromagnètic.
* **Cas B:** Connectar $20$ ordinadors de taula en una mateixa aula d'informàtica d'un institut a baix cost (distància màxima $20\text{ metres}$).
* **Cas C:** Connectar un auricular sense fils a un telèfon mòbil per escoltar música en una xarxa d'àrea personal (PAN).
* **Cas D:** Rebre la transmissió continuada d'un programa de ràdio en un receptor d'automòbil mentre es circula per la carretera.

---

## Apartat 2: Senyals, Pertorbacions i Característiques Físiques

### Exercici 3: Qüestions tècniques sobre pertorbacions

Respon breument a les següents preguntes sobre la qualitat de la transmissió:

1. Quina diferència hi ha entre un cable UTP i un cable STP? En quin entorn està justificat l'ús del segon?
2. Defineix el concepte d'atenuació i explica com afecta la distància a la qualitat del senyal.
3. Per quina raó la fibra òptica no pateix interferències de tipus electromagnètic (EMI) a diferència dels cables de coure?

---

## Apartat 3: Càlculs de Velocitat i Temps de Descàrrega

Aplica la fórmula general de descàrrega per als següents problemes:

$$\text{Temps de descàrrega (s)} = \frac{\text{Mida de l'arxiu (bits)}}{\text{Velocitat de transmissió (bps)}}$$

### Exercici 4: Càlculs directes de temps de transferència

* **Problema A:** Es vol descarregar un arxiu de vídeo de $3\text{ GB}$ mitjançant una connexió de fibra òptica de $300\text{ Mbps}$. Quants segons trigarà la descàrrega completant la conversió binària ($1\text{ GB} = 1024^3\text{ Bytes}$)?
* **Problema B:** Una càmera d'un sistema de seguretat envia una imatge de $4\text{ MB}$ a un servidor central a través d'un enllaç de $5\text{ Mbps}$. Quin és el temps exacte que triga a transferir-se la imatge?

---

### EXTRA Exercici 5: Càlculs amb pertorbacions del mitjà (Soroll i Atenuació)

* **Problema A (Cable elèctric amb soroll):** Una connexió per cable UTP Cat 6 té una velocitat nominal de $1\text{ Gbps}$ ($1000\text{ Mbps}$). A causa del soroll elèctric d'un motor pròxim, la velocitat efectiva es redueix un $20\%$. Quant trigarà a transferir-se un fitxer de $10\text{ GB}$?
* **Problema B (Senyal de ràdio amb atenuació):** Un dispositiu connectat per xarxa sense fils (WLAN) rep un senyal amb una atenuació del $35\%$ a causa de les parets de l'edifici. Si la velocitat nominal de la xarxa és de $100\text{ Mbps}$:
  1. Quina serà la velocitat efectiva de la connexió?
  2. Quants segons seran necessaris per descarregar un arxiu de $2\text{ GB}$?