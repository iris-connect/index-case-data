# iCWA Konzeptbestandteile


## Akteure:

### Indexperson (IP)

Eine erkrankte Person, die auf COVID-19 getestet wird und wegen eines positiven Tests isoliert werden muss.

### Gesundheitsamt (GA)

Das für die Betreuung der Indexperson zuständige Gesundheitsamt.


## Softwareakteuere:

### Corona-Warn-App (CWA)
Die Corona-Warn-App der Indexperson

### IRIS Client (IRIS) 
Der IRIS Client im Gesundheitsamt, der entsprechende Daten entgegennehmen kann.

## Datenstrukturen:

### Fallinformationen (FI)
Zur Indexperson gehörende Informationen wie etwa der Impfstatus sowie der Symptombeginn der Erkrankung

Mögliche hilfreiche Fallinformationen:
#### Symptombeginn
Angabe des Symptombeginns in Relation zu Test.

#### Impfstatus
Abbildung in SORMAS / anderen Anwendungen über mögliches Matching mit Impfzertifikat

- Anzahl Impfungen
- Datum erste Impfung
- Datum letzte Impfung
- Impfstoffname (der letzten Impfung?)


#### Genesenenzertifikat
Bei Vorhandensein eines Genesenenzertifikats ist von einer Reinfektion auszugehen, wenn diese einen entsprechenden Zeitraum seit der letzten Infektion zurückliegt.

#### weitere mögliche Datenpunkte 
Die folgenden Datenpunkte wären aus Sicht der IP für die weitere Statistik möglich, sind aber nicht Teil der Basisdaten der CWA
- Symptome 


### Kontaktinformationen (KI)
Kontaktpersonen oder Orte zu denen die Indexperson im relevanten Zeitraum Kontakt hatte, idealerweise bereits gepflegt im Kontakttagebuch der CWA. Diese Informationen können aber auch vor der Übermittlung ergänzt werden.

#### Informationen zu Kontaktpersonen
- Name
- Telefon 
- E-Mail
- Datum letzter Kontakt
- Notizen / Kommentar

#### Ereignis
- Bezeichnung
- Ort
- Datum
- Notizen / Kommentar

## grober Ablauf
1. Eine Indexperson IP registriert in ihrer CWA einen Test und wartet auf ihr Testergebnis
2. Die IP kann bereits bei registriertem Test ihr Kontakttagebuch aufbereiten oder ergänzen sowie ihre Fallinformationen aufbereiten
3. Die IP erhält über die CWA ihr positives Testergebnis
4. Die IP teilt ihr positives Testergebnis über die CWA mit ihren Risikokontakten und löst so Warnungen bei den Kontakten aus
5. Die IP bestimmt dann über Eigabe der Postleitzahl ihr zugehöriges Gesundheitsamt
6. Die IP teilt nun entweder ihre vorbereiteten Daten mit dem GA oder legt die Fallinformationen und Kontaktinformationen in diesem Schritt an und teilt sie mit ihrem GA
7. Die IP erhält einen verständlichen Token nach Übermittlung ihrer Fallinformationen und Kontaktinformationen
8. Das GA kontaktiert die IP und bekommt den Token, mit sie in IRIS die digital übermittelten Fall- und Kontaktinformationen zuordnen und in die IfSG-Fachwendung übertragen kann.

## Rahmenbedingungen
- Der Prozess ist in allen Teilen ein freiwilliger Prozess
- Die IP kann alle zu übermittelnden Daten vor Übermittlung prüfen und Teile der Daten explizit nicht freigeben
