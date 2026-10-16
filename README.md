 Simulador de la Llei D'Hondt — Província de València

## 1. Descripció del projecte

Aquest projecte consisteix en el desenvolupament d'una pàgina web que permet simular l'assignació de diputats de la província de València mitjançant la llei D'Hondt.

L'objectiu és crear una eina interactiva que facilite la comprensió del sistema electoral espanyol i permeta comprovar com es distribueixen els escons entre els diferents partits polítics en funció dels vots obtinguts.

La web permet modificar tant el nom dels partits polítics com el nombre de vots de cadascun, de manera que es poden provar diferents escenaris electorals i observar com afecten al repartiment dels diputats.

## 2. Objectius

Els objectius principals del projecte són:

- Implementar el sistema d'assignació de diputats mitjançant la llei D'Hondt.
- Permetre editar el nom de cada partit polític.
- Permetre modificar el nombre de vots obtinguts per cada partit.
- Mostrar els resultats del repartiment dels escons de manera clara i visual.
- Facilitar la simulació de diferents resultats electorals.
- Ajudar a comprendre el funcionament del sistema electoral a través de la interacció amb la web.

## 3. Funcionament de la llei D'Hondt

La llei D'Hondt és un mètode matemàtic utilitzat en les eleccions al Congrés dels Diputats d'Espanya per distribuir els escons entre les candidatures electorals.

En el cas de la província de València, s'ha de tindre en compte el nombre de diputats que li corresponen en la convocatòria electoral corresponent.

El procediment és el següent:

1. Cada partit obté un nombre determinat de vots.
2. Els vots de cada partit es divideixen entre 1, 2, 3, 4 i així successivament.
3. Es recopilen els quocients resultants de totes les candidatures que poden participar en el repartiment.
4. S'ordenen els quocients de major a menor.
5. S'assigna un escó a cadascun dels quocients més alts fins a completar el nombre total de diputats que s'han de repartir.

D'aquesta manera, el nombre d'escons de cada partit depén dels seus vots i de la distribució dels vots entre la resta de candidatures.

### Exemple

Suposem que participen tres partits en una simulació:

| Partit | Vots |
|---|---:|
| Partit A | 100.000 |
| Partit B | 70.000 |
| Partit C | 40.000 |

Per aplicar la llei D'Hondt, dividim els vots de cada partit entre 1, 2, 3 i els divisors següents que siguen necessaris.

| Partit | ÷ 1 | ÷ 2 | ÷ 3 |
|---|---:|---:|---:|
| Partit A | 100.000 | 50.000 | 33.333 |
| Partit B | 70.000 | 35.000 | 23.333 |
| Partit C | 40.000 | 20.000 | 13.333 |

Els escons s'assignen seguint l'ordre dels quocients més alts fins a completar el nombre de diputats disponibles.

Aquest exemple és únicament il·lustratiu i no representa els resultats d'unes eleccions reals.

## 4. Funcionalitats de la web

### 4.1. Edició dels partits polítics

L'usuari pot modificar el nom dels partits que apareixen en la simulació.

Aquesta funcionalitat permet adaptar l'aplicació a diferents candidatures o utilitzar noms genèrics per a fer proves.

### 4.2. Modificació del nombre de vots

L'usuari pot introduir o modificar el nombre de vots obtinguts per cada partit.

Quan es modifica aquesta informació, el sistema pot recalcular el repartiment dels diputats per mostrar els resultats corresponents a les noves dades.

### 4.3. Càlcul automàtic dels escons

La web aplica la fórmula D'Hondt a les dades introduïdes.

El sistema calcula els quocients de cada partit, identifica els més alts i assigna els escons corresponents fins a completar el nombre total de diputats de la circumscripció.

### 4.4. Visualització dels resultats

Els resultats es mostren de manera que l'usuari puga identificar fàcilment:

- El nom de cada partit.
- El nombre de vots obtinguts.
- El nombre de diputats assignats.
- La distribució final dels escons.

Aquesta representació facilita la comparació entre candidatures i permet observar com els canvis en els vots afecten el resultat electoral.

## 5. Requisits i consideracions

Perquè la simulació siga coherent amb el sistema electoral real, cal tindre en compte les condicions següents:

- El nombre total de diputats que s'han de repartir ha de correspondre al nombre d'escons assignats a la província de València en la convocatòria electoral seleccionada.
- Els vots introduïts han de ser nombres enters no negatius.
- Els camps de votació han de validar les dades abans de fer els càlculs.
- Només s'han d'assignar els escons disponibles.
- Les candidatures han de participar en el repartiment d'acord amb els requisits de la legislació electoral aplicable.
- En cas d'empat entre quocients, s'ha d'aplicar el criteri establit per la normativa electoral.

En les eleccions al Congrés dels Diputats, la Llei orgànica del règim electoral general estableix un llindar mínim del 3 % dels vots vàlids emesos en la circumscripció per a participar en l'assignació d'escons.

Per tant, si es vol reproduir fidelment el sistema electoral real, la web ha de comprovar aquest requisit abans d'aplicar la fórmula D'Hondt.

## 6. Tecnologies utilitzades

Les tecnologies dependran de la implementació concreta de la pàgina web.

Una possible solució és utilitzar:

- **HTML:** per a definir l'estructura de la pàgina.
- **CSS:** per a dissenyar i organitzar visualment els elements.
- **JavaScript:** per a gestionar les dades introduïdes, aplicar la fórmula D'Hondt i actualitzar els resultats.

Aquestes tecnologies permeten desenvolupar una aplicació web interactiva sense necessitat d'un servidor per a efectuar els càlculs bàsics.

## 7. Ús de la intel·ligència artificial

Per al desenvolupament del projecte s'utilitza una eina d'intel·ligència artificial com a suport en el disseny i la implementació de la pàgina web.

La IA pot ajudar a:

- Proposar l'estructura inicial de la web.
- Generar el codi HTML, CSS i JavaScript.
- Implementar l'algoritme de repartiment d'escons.
- Detectar errors en els càlculs.
- Millorar la presentació visual dels resultats.
- Preparar exemples per a comprovar el funcionament de l'aplicació.

El resultat generat s'ha de revisar i provar per a verificar que els càlculs siguen correctes i que el comportament de la web s'ajuste als requisits del projecte.

## 8. Proves de funcionament

Per a comprovar el funcionament de l'aplicació, es poden realitzar les proves següents:

1. Introduir un conjunt de vots per a diversos partits i verificar que el nombre total de diputats assignats coincideix amb el nombre d'escons disponibles.
2. Canviar el nom d'un partit i comprovar que la modificació apareix correctament en els resultats.
3. Modificar els vots d'un partit i comprovar que el repartiment es recalcula.
4. Introduir zero vots per a una candidatura i verificar que no rep cap escó.
5. Introduir valors negatius o dades no numèriques i comprovar que el sistema les rebutja.
6. Provar situacions en què dos o més partits tinguen quocients iguals.
7. Comprovar que les candidatures que no arriben al llindar legal no participen en el repartiment, si aquesta funcionalitat està implementada.

## 9. Resultat esperat

El resultat final és una pàgina web interactiva que permet simular l'assignació de diputats de la província de València mitjançant la llei D'Hondt.

L'usuari pot editar els noms dels partits, modificar els seus vots i consultar la distribució dels escons resultant.

Així, el projecte combina la programació web amb l'aplicació d'un procediment matemàtic real, i ofereix una eina pràctica per a entendre millor el funcionament del sistema electoral.

## 10. Conclusió

Aquest projecte permet comprendre de manera pràctica com s'aplica la llei D'Hondt al repartiment dels diputats.

La possibilitat de modificar els partits i els vots facilita l'experimentació amb diferents escenaris i ajuda a observar que la distribució dels escons no depén únicament del percentatge de vots de cada candidatura, sinó també dels resultats de la resta de partits.

La web constitueix, per tant, una eina educativa i interactiva per a estudiar el sistema electoral i la representació política de la província de València.
