# SESSIÓ 3
# 🛠️ FITXA DE TREBALL
**Unitat Operativa:** NetWorking Solutions | **Mòdul:** 0225  
**Alumnat / Equip:** ____________________________________ **Data:** ____________

---

## 📄 TALLER 1: Encapsulació en els Models OSI i TCP/IP (1 hora)

### 1. Marc Teòric de Consulta Ràpida

| Capa OSI | Nom Capa OSI | Equivalència TCP/IP | PDU (Unitat de Dades) | Direccionament / Capçalera Clau |
| :---: | :--- | :--- | :--- | :--- |
| **7** | Aplicació | Aplicació | Dades | Protocol d'aplicació (HTTP, SSH, DNS...) |
| **6** | Presentació | Aplicació | Dades | Format i xifrat (SSL/TLS, ASCII...) |
| **5** | Sessió | Aplicació | Dades | Gestió de diàleg i connexió |
| **4** | Transport | Transport | **Segment** | Ports origen i destinació (TCP / UDP) |
| **3** | Xarxa | Internet | **Paquet** | Adreces IP origen i destinació |
| **2** | Enllaç de Dades | Accés a la Xarxa | **Trama** | Adreces MAC origen i destinació |
| **1** | Física | Accés a la Xarxa | **Bits** | Senyals elèctrics, òptics o ones |

---

### 2. Pràctica: La Dinàmica dels Sobres (Simulació d'Encapsulació)

#### 🎯 Objectiu del Repte
Simular el viatge d'una petició web (`HTTP GET /index.html`) des del vostre ordinador (Client) fins a un servidor, preparant les capçaleres d'encapsulació pas a pas des de la Capa d'Aplicació fins a la Capa Física.

#### ✂️ Instruccions d'Execució
1. **Sobret 1 (Dades / Aplicació):** Escriviu el missatge `"PETICIÓ HTTP GET"` en un paper prim i fiqueu-lo al sobre més petit.
2. **Sobret 2 (Segment TCP / Capa 4):** A l'exterior del sobre 1, escriviu el port origen (ex: `Port 49152`) i el port destinació (ex: `Port 80`). Fiqueu el sobre 1 dins del sobre 2.
3. **Sobret 3 (Paquet IP / Capa 3):** A l'exterior del sobre 2, escriviu la IP origen (ex: `192.168.1.50`) i la IP destinació (ex: `142.250.184.206`). Fiqueu el sobre 2 dins del sobre 3.
4. **Sobret 4 (Trama MAC / Capa 2):** A l'exterior del sobre 3, escriviu la MAC origen (`AA:BB:CC:11:22:33`) i la MAC destinació (`DD:EE:FF:44:55:66`). Fiqueu el sobre 3 dins del sobre 4.
5. **Capa 1 (Física):** Dibuixeu una seqüència de 0 i 1 a la solapa del sobre exterior per representar la conversió a senyal físic.

---

### ✍️ Preguntes de Consolidació (Taller 1)
*Respon aquestes qüestions per adjuntar al teu Diari del Tècnic:*

1. **Desencapsulació:** Quan el servidor rep el sobre físic, en quin ordre va obrir els sobres i quina informació comprova primer?  
   ____________________________________________________________________________________________________

2. **Diagnòstic d'Avaries:** Si un router de frontera rep la trama però la IP destinació no existeix a les seves taules, a quina capa de la PDU ha hagut de mirar per prendre la decisió?  
   ____________________________________________________________________________________________________

---

---

## 🔬 TALLER 2: Autòpsia de Maquinari de Xarxa (1 hora)

### 1. Formulari d'Anàlisi d'Equips

Inspeccioneu els dispositius físics assignats al vostre banc de treball (o les seves fitxes tècniques/fotografies detallades) i completeu la següent taula d'inspecció:

| Equip ID | Nom del Dispositiu | Nombre de Ports / Interfícies | Capa OSI d'Actuació (1, 2, 3 o 4-7) | Quin tipus d'adreça mira per reenviar? (MAC / IP / Cap) |
| :---: | :--- | :---: | :---: | :--- |
| **EQ-01** | *Ex. Hub antic de 8 ports* | 8 ports RJ45 | Capa 1 | Cap (Repeteix el senyal a tots els ports) |
| **EQ-02** | | | | |
| **EQ-03** | | | | |
| **EQ-04** | | | | |

---

### 2. Estudi de Casos i Resolució de Problemes

Llegiu els següents escenaris tècnics i determineu quin equip cal utilitzar en cada cas, justificant la decisió segons la seva capa d'actuació:

#### 📋 Escenari A: "L'Aula Saturada"
> *Un conjunt de 10 ordinadors estan connectats a un dispositiu antic. Quan dos ordinadors envien informació alhora, la xarxa es col·lapsa i les transmissions s'aturen constantment per col·lisió.*

* **De quin equip es tracta?** ____________________________________________________
* **A quina capa actua?** _______________________________________________________
* **Amb quin dispositiu modern el substituiries per evitar les col·lisions?** ____________________

---

#### 📋 Escenari B: "Connexió entre Departaments"
> *L'equip de Desenvolupament (Xarxa `192.168.10.0/24`) necessita enviar fitxers a l'equip de Comptabilitat (Xarxa `192.168.20.0/24`). Tot i estar connectats al mateix switch, no aconsegueixen comunicar-se.*

* **Per què un switch de Capa 2 no pot resoldre aquesta comunicació per si sol?**  
  ____________________________________________________________________________________________________
* **Quin dispositiu de Capa 3 cal afegir per interconnectar les dues subxarxes?** ____________________

---

### 📥 Lliurament i Evidència
Preneu una fotografia de l'equip analitzat al Taller 1 i de la dinàmica de sobres del Taller 2, i enganxeu-les a la secció d'**Evidències Fotogràfiques** de la fitxa de la Sessió 3 del vostre **Diari del Tècnic**.