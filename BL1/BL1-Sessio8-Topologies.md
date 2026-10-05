# Topologies de Xarxa: Activitats

## Apartat 1: Identificació i Conceptes de Topologies

### Exercici 1: Reconeixement de Topologies

Relaciona la descripció amb la topologia de xarxa corresponent (**Bus, Anell, Estrella, Malla Total, Arbre**):

1. Tots els nodes es connecten a un únic canal o cable central mitjançant terminadors a cada extrem.
2. Tots els dispositius es connecten directament a un punt central comú (com ara un switch o un concentrador).
3. Cada node està connectat directament amb tots els altres nodes de la xarxa, oferint la màxima redundància.
4. Els nodes es connecten formant un cercle tancat on el senyal circula en una sola direcció d'un node al següent.
5. Estructura jeràrquica formada per la combinació o interconnexió de múltiples estrelles.

---

### Exercici 2: Detecció d'errors en afirmacions

Analitza les següents afirmacions sobre topologies i indica si són **VERTADERES** o **FALSES**. Justifica breument la resposta en cas de ser falsa:

* **a)** En una topologia en bus, si un ordinador personal s'apaga, tota la xarxa deixa de funcionar immediatament.
* **b)** La topologia en estrella és molt resistent a la fallada d'un cable individual que connecta un ordinador de client.
* **c)** La topologia en malla total és la solució més econòmica de cablejar quan tenim 30 ordinadors a la mateixa aula.
* **d)** En una topologia en anell simple, el trencament del cable principal en qualsevol punt no afecta la comunicació entre la resta de nodes.

---

## Apartat 2: Anàlisi de Fallades, Resiliència i Càlculs

### Exercici 3: Matriu d'impacte davant d'incidents

Completa la taula indicant quina repercussió té en el conjunt de la xarxa cadascun dels dos tipus d'incidents segons la topologia utilitzada:

| Topologia | Tall en un cable d'un equip individual | Fallada del dispositiu o canal central |
| --- | --- | --- |
| **Bus** |  |  |
| **Estrella** |  |  |
| **Anell** |  |  |
| **Malla Total** |  |  |

---

### Exercici 4: Càlcul de connexions en Malla Total

Per calcular el nombre d'enllaços o cables ($N_{cables}$) necessaris per interconnectar $n$ equips en una topologia de malla total s'utilitza la fórmula:

$$N_{cables} = \frac{n \cdot (n - 1)}{2}$$

Calcula i respon:

1. Quants cables es necessiten per connectar $6$ servidors crítics en una topologia de malla total?
2. Si una oficina vol connectar $20$ ordinadors en malla total, quants cables necessitarà?
3. A partir del resultat anterior, explica per què no és habitual utilitzar la topologia en malla total en xarxes LAN d'oficina o d'aula.

---

## Apartat 3: Casos Pràctics d'Aplicació

### Exercici 5: Selecció de la millor topologia

Tria la topologia més adient per a cadascun dels escenaris i justifica la teva resposta:

* **Cas A:** Un centre de dades (*Data Center*) bancari que requereix alta disponibilitat i no es pot permetre la caiguda de la xarxa en cap dels seus $5$ servidors principals.
* **Cas B:** Una aula d'informàtica d'un institut on es vol centralitzar el control de la xarxa en un switch per poder afegir o treure ordinadors de manera fàcil i ràpida.
* **Cas C:** Una xarxa d'un edifici d'oficines de tres plantes on cada planta té el seu propi switch central i tots tres switchs es connecten a un switch principal d'edifici.
