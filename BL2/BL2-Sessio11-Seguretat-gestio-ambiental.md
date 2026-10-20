# BL2. A1 - Medis de transmissió i rosetes

# SESSIÓ 11: Seguretat i gestió ambiental
---

## 📖 1. Marc Normatiu i Marc Curricular

Aquest bloc teòric dona compliment directe al **Resultat d'Aprenentatge 6 (RA6)** del mòdul **0225 (Xarxes Locals)**: *Compleix les normes de prevenció de riscos laborals i de protecció ambiental, identificant els riscos associats i les mesures de protecció.*

### Marcs Legals de Referència:
* **Llei 31/1995**, de Prevenció de Riscos Laborals.
* **RD 486/1997**, sobre disposicions mínimes de seguretat i salut als llocs de treball.
* **RD 488/1997**, sobre disposicions mínimes relogioses a treball amb equips que inclouen pantalles de visualització.
* **RD 110/2015**, sobre residus d'aparells elèctrics i electrònics (RAEE).

---

## ⚡ 2. Prevenció de Riscos Laborals (PRL) en Infraestructures de Xarxa

L'activitat de muntatge, cablejat, manteniment i configuració d'equips de comunicació comporta una sèrie de riscos específics que cal identificar i prevenir.

### 2.1. Classificació de Riscos i Mesures Preventives

| Tipus de Risc | Origen / Tasca Associada | Mesures Preventives i Bones Pràctiques |
| :--- | :--- | :--- |
| **Risc Elèctric** | Manipulació d'armaris Rack, servidors, SAIs, fonts d'alimentació o instal·lació de preses de corrent. | • Comprovar la presa de terra en bastidors i xassís metàl·lics.<br>• Utilitzar eines aïllades i homologades.<br>• Prohibició absoluta de manipular equips oberts sota tensió.<br>• Desconnectar la font d'alimentació abans d'instal·lar Targetes NIC o mòduls intern. |
| **Riscos Mecànics i d'Eines** | Tall de canaletes de PVC, ús de bisturís, eines de crimpació, inserció LSA/110 i serres. | • Mantenir les eines de tall en bon estat i amb la protecció posada.<br>• Fer el tall de canaleta sobre superfícies estables, mai sobre la mà o la cama.<br>• Utilitzar eines d'impacte homologades evitant l'ús de la força bruta. |
| **Riscos de la Fibra Òptica** | Fusió, pelat i connectorització de cables de fibra òptica. | • **Risc ocular:** Mai mirar directament l'extrem d'una fibra ni un port SFP/GBIC (radiació làser invisible).<br>• **Risc per estelles:** Les restes de nucli de vidre poden penetrar a la pell o als ulls.<br>• Utilitzar ulleres de protecció i no menjar ni beure a la zona de treball. |
| **Ergonomia i Càrregues** | Transport i muntatge d'armaris Rack, servidors de gran format, SAIs i bateries. | • Flexionar els genolls i mantenir l'esquena recta en aixecar pesos (>15-20 kg).<br>• Demanar ajuda a un company per al muntatge de bastidors o equips pesats al Rack.<br>• Mantenir postures neutres en el passatge de cable en sostres o canals. |
| **Caigudes i Ensopegades** | Desordre a l'aula/laboratori, cables escampat per terra, treballs en alçada (escala). | • Mantenir el banc de treball i les zones de pas lliures de cables penjants o eines.<br>• Utilitzar escales de mà homologades amb topes antilliscants i suport estable. |

---

### 2.2. Equips de Protecció Individual (EPIs)

En els tallers pràctics i entorns reals de treball és obligatori l'ús dels següents EPIs segons la tasca:

* 👓 **Ulleres de seguretat homologades:** Obligatòries durant el tall de canaletes de PVC, tall de cablejat i operacions de pelat, tall i fusió de fibra òptica.
* 🧤 **Guants de protecció mecànica:** Per a la manipulació de bastidors metàl·lics, xassís amb cantells vius, eines de tall i passat de cables per canalitzacions.
* 👞 **Calçat de seguretat:** Recomanat durant el transport, desplaçament i muntatge d'armaris Rack, SAIs i servidors de gran pes.

---

## ♻️ 3. Gestió Mediambiental i Tractament de Residus (RAEE)

Els equips de xarxa i els materials utilitzats en el seu desplegament generen residus que tenen un fort impacte ambiental si no es gestionen adequadament.

### 3.1. Gestió de Residus d'Aparells Elèctrics i Electrònics (RAEE)

Segons el **RD 110/2015**, els equips informàtics i de telecomunicacions s'han de classificar i lliurar a gestors de residus autoritzats.

# ACTIVITATS

# 📦 NETWORKING SOLUTIONS — DOSSIER DE PREVENCIÓ I SOSTENIBILITAT
**Mòdul Professional:** 0225 Xarxes Locals - RA 6
**Cicle Formatiu:** Sistemes Microinformàtics i Xarxes (SMX)  

---

## 📄 FITXA DE TREBALL 1: AUDITORIA DE SEGURETAT (PRL) A L'AULA-LABORATORI

**Data d'execució:** ____ / ____ / 20__  
**Equip d'Auditoria / Alumnat:** ____________________________________________________  
**Lloc d'Auditoria:** Laboratori de Xarxes   

---

### 1. Marc Teòric de Consulta Ràpida (PRL)
* **Contacte Elèctric:** Atenció amb els connectors de xarxa actius, SAIs (Sistemes d'Alimentació Ininterrompuda) i xassís metàl·lics d'armaris rack sense presa de terra.
* **Riscos Mecànics:** Manipulació d'eines tallants (bisturís, guillotines, eines d'impacte 110/LSA) i tall de canaletes de PVC.
* **Fibra Òptica:** Risc per radiació invisible en transceptors (làser/LED) i risc d'inserció de fragment de nucli de vidre en pell o ulls.

---

### 2. Registre de Situacions de Risc i Mesures Correctores

Inspeccioneu la zona de treball i analitzeu els 3 escenaris assignats. Empleeu la matriu per registrar les dades:

#### 📋 Escenari A: Zona de l'Armari Rack
* **Situació:** Un tècnic està connectant un Switch a un SAI en marxa mentre passa cables per la zona de pas, deixant-los penjant a l'alçada dels peus.
* **Tipus de Risc:** ____________________________________________________________________
* **Mesura Preventiva / Correctora:** ___________________________________________________
_________________________________________________________________________________________

#### 📋 Escenari B: Zona de Treball amb Fibra Òptica
* **Situació:** Un integrador retalla la coberta i el nucli de fibra òptica, bufant les restes de vidre sobre la taula i mirant directament pel connector SFP per veure si "passa llum".
* **Tipus de Risc:** ____________________________________________________________________
* **Mesura Preventiva / Correctora:** ___________________________________________________
_________________________________________________________________________________________

#### 📋 Escenari C: Canalització i connexions
* **Situació:** Es procedeix a tallar canaleta de PVC amb serra manual sense utilitzar ulleres i s'aplica força amb l'eina d'impacte agafant la roseta RJ-45 amb la mà oposada.
* **Tipus de Risc:** ____________________________________________________________________
* **Mesura Preventiva / Correctora:** ___________________________________________________
_________________________________________________________________________________________

---

### 3. Matriu d'Equips de Protecció Individual (EPIs)

Seleccioneu amb una **[X]** els EPIs que son d'obligat compliment segons la tasca tècnica realitzada:

| Tasca Tècnica a Realitzar | Ulleres de Protecció | Guants Mecànics / Antitall | Calçat de Seguretat | Mascareta / Prot. Auditiva |
| :--- | :---: | :---: | :---: | :---: |
| **Tall, pelat i fusió de Fibra Òptica** | [ ] | [ ] | [ ] | [ ] |
| **Muntatge i transport d'un Armari Rack (42U)** | [ ] | [ ] | [ ] | [ ] |
| **Tall de canaletes de PVC amb serra/guillotina** | [ ] | [ ] | [ ] | [ ] |
| **Crimpats i inserció de cable UTP a rosetes** | [ ] | [ ] | [ ] | [ ] |

---

## 📄 FITXA DE TREBALL 2: TRIATGE DE RESIDUS (RAEE) I ECONOMIA CIRCULAR

**Data d'execució:** ____ / ____ / 20__  
**Tècnic/a en Gestió Mediambiental:** ______________________________________________  
**Lloc de Triatge:** Zona de Reciclatge / Taller de Sistemes  

---

### 1. Marc Teòric de Consulta Ràpida (RAEE)
* **Reial Decret 110/2015 (RAEE):** Obliga a la recollida selectiva, segregació i traçabilitat dels aparells elèctrics i electrònics.
* **Coure i Metalls:** Material altament reciclable que s'ha de separar de la resta de plàstics/polímers.
* **Residus Perillosos (RP):** Bateries de plom-àcid (SAIs), piles de liti (plaques mare) i nuclis de vidre (fibra).

---

### 2. Matriu de Segregació de Materials i Deixalles

L'empresa ha fet neteja de la sala de servidors. Classifiqueu cada element dipositant-lo conceptualment en el contenidor corresponent:

| # | Element / Residu Generat | Contenidor Blau (Paper/Cartró) | Contenidor Groc (Plàstic/PVC) | Contenidor Coure / Metalls | Contenidor Rígid Específic | Punt Verd / RAEE (Electrònica/Bateries) |
|---| :--- | :---: | :---: | :---: | :---: | :---: |
| **1** | Retalls de cable de xarxa UTP (Coure) | [ ] | [ ] | [ ] | [ ] | [ ] |
| **2** | Restes de nucli de vidre de fibra òptica | [ ] | [ ] | [ ] | [ ] | [ ] |
| **3** | Trossos de canaleta de PVC i brides de plàstic | [ ] | [ ] | [ ] | [ ] | [ ] |
| **4** | Bateria de plom usada d'un SAI | [ ] | [ ] | [ ] | [ ] | [ ] |
| **5** | Caixes de embalatge dels switches nous | [ ] | [ ] | [ ] | [ ] | [ ] |
| **6** | Placa electrònica d'un router avariat | [ ] | [ ] | [ ] | [ ] | [ ] |
| **7** | Connectors RJ-45 de plàstic defectuosos | [ ] | [ ] | [ ] | [ ] | [ ] |
| **8** | Xassís metàl·lic d'un servidor antic | [ ] | [ ] | [ ] | [ ] | [ ] |

---

### 3. Pla d'Economia Circular i Reutilització Tècnica

Respondreu a les següents qüestions de millora ambiental de la infraestructura:

1. **Reutilització d'Equips Obsolets:** Us han lliurat un *Switch FastEthernet (10/100 Mbps)* de 24 ports antic que ja no serveix per a la xarxa principal. Proposeu **dues utilitats pràctiques** abans d'enviar-lo directament a reciclatge:
   * **Ús 1:** __________________________________________________________________________
   * **Ús 2:** __________________________________________________________________________

2. **Seguretat i Medi Ambient en Fibra Òptica:** Per què és un error greu llençar les restes de retalls de fibra òptica a les papereres convencionals de plàstic o paper?
   _____________________________________________________________________________________
   _____________________________________________________________________________________

3. **Eficiència Energètica (Green IT):** Indiqueu 2 mesures de configuració o manteniment en els equips de xarxa per reduir el consum elèctric de la instal·lació:
   * **Mesura 1:** ______________________________________________________________________
   * **Mesura 2:** ______________________________________________________________________