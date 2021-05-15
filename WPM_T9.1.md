# Aufgabe MALIS 20.3 WPM_T9.1

Autorin: Chantal F. Köppl

# Datenintensive bzw. datenfokussierte Prozesse und Möglichkeiten der Prozessoptimierung in der Gemeinsamen Normdatei (GND) - eine Auswahl

Die Gemeinsame Normdatei ([GND](https://www.dnb.de/DE/Professionell/Standardisierung/GND/gnd_node.html)) ist ein von den Bibliotheken im D-A-CH-Raum kooperativ gepflegtes Normdatenhub. In ihr wurden 2012 vier vorher bestehende, einzelne Normdateien zusammengeführt. Die folgende Zusammenstellung zeigt auszughaft einige Beispiele für datenintensive bzw. datenfokussierte Prozesse in der GND und beschreibt im gleichen Zuge Möglichkeiten zur Optimierung dieser Prozesse.

# Datenintensive bzw. datenfokussierte Prozesse in der GND

Die Arbeit an der GND besteht aus vielen unterschiedlichen Facetten. Es wird in diesem Rahmen nicht möglich sein, auf alle Aspekte einzugehen, daher erfolgt hier eine (nicht repräsentative) Auswahl von Themenbereichen und von insgesamt sieben mit ihnen verknüpften Prozessen.


## Prozesse im Zusammenhang mit der Erschließung

### 1. Erschließung von Medien
Die Prozesse zur Erschließung von Medien sind mit jenen der Normdatenerschließung eng verknüpft, wenn es um die maschinelle Unterstützung meist intellektuell vollzogener Arbeitsschritte geht. Das Anlegen und Pflegen von Titeldatensätzen zur formalen und inhaltlichen Erfassung von Medien ist ressourcenintensiv und wird daher zunehmend mithilfe von Automatisierungsverfahren unterstützt. Dazu gehört beispielsweise, dass Titeldatensätze durch maschinelle Beschlagwortung, Klasifikation oder Spracherkennung / Vergabe von Sprachencodes angereichert werden. Dabei werden computerlinguistische Verfahren eingesetzt, die die vorhandenen Metadaten, Volltexte oder Tables of Contents auslesen bzw. statistisch auswerten, mit dem jeweiligen Zielvokabular (GND, DDC ...) abgleichen und die betreffenden IDs, Terme und Notationen in den Titeldatensatz übernehmen. Auf die maschinelle Normdatensatzverknüpfung wird noch einmal anhand eines konkreteren Beispiels unter Punkt 3 eingegangen. Schließlich dienen die genannten Verfahren auch dazu, Parallelabgleiche vorzunehmen. Ziel der Parallelabgleiche ist es, die Datensätze von Titeln, die sowohl als Print- als auch als Onlinepublikation vorliegen, miteinander zu verknüpfen und die Metadaten der Inhaltserschließung wechselseitig auszutauschen. An der Deutschen Nationalbibliothek ist die Abteilung AEN (Automatische Erschließung von Netzpublikationen) für die Erarbeitung und Weiterentwicklung solcher Verfahren zuständig.
Noch immer können diese Verfahren die intellektuelle Arbeit nur unterstützen, nicht aber (vollständig) ablösen. Daher ist es notwendig, die maschinell angereicherten Daten regelmäßig durch intellektuelle Stichproben zu überprüfen.

### 2. Regelwerksänderungen
Sämtliche Einträge in die GND werden nach dem gemeinsamen Regelwerk [RDA](https://www.dnb.de/DE/Professionell/Standardisierung/Standards/_content/rda_akk.html) angelegt. Hin und wieder kommt es dazu, dass Teile des Regelwerks überarbeitet werden und Katalogisierer+innen und GND-Redakteur+innen die entsprechenden Felder nach einer neuen Regel befüllen müssen.
Ab dem Geltungszeitpunkt des neuen oder aktualisierten Regelwerks werden alle neuen Katalogisate oder Normdatensätze nach den neuen Regeln angelegt, während die vorherigen Daten in der Regel bestehen bleiben. Stößt ein+e Katalogisierer+in oder ein+e Redakteur+in bei seiner Arbeit auf einen nach altem Regelwerk angelegten Datensatz, so passt er diesen händisch an das neue Regelwerk an. Eine Regelwerksänderung hat darum immer eine heterogene, nicht ganz konsistente Datenlage bzw. Erfassungslage zur Folge, die nur nach und nach als work in progress bereinigt wird. 
Es wäre denkbar, die Aktualisierung der Datensätze auf das neue Regelwerk teilweise  maschinell zu unterstützen. Dazu müsste zunächst die Art der Änderung des Regelwerks ausgewertet werden, indem die neue und die alte Version des Regelwerks miteinander verglichen werden. Es müsste weiterhin festgestellt werden, welche Metadatenfelder von der Änderung betroffen sind und in welchem Format diese befüllt sind, um dann entsprechend des neuen Regelwerks ein Zielformat festzulegen.
In diesem Zuge könnte man auch darüber nachdenken, ein solches Verfahren mit einer maschinell unterstützen "Prüfung" der Regelkonformität bestimmter Felder zu verbinden. Denn auch hier wäre ein Schema, ein Format oder eine Syntax festzulegen, nach denen die Felder jeweils mit kontrollierten Werten oder Literalen zu besetzen sind.

3. Erschließung und Verknüpfung von Normdaten
Die in Titeldaten genannten Personen wie beispielsweise Autoren oder Herausgeber sind häufig nicht mit Personennormdaten der GND, sogenannten Tp-Sätzen, verknüpft. Wie im Fall der Regelwerksänderung ist man auch hier darauf angewiesen, dass ein+e Katalogisierer+in den Datensatz im Rahmen anderer Arbeiten aufruft, die fehlende Verknüpfung erkennt und behebt.
Im Fall von Personen, aber auch von Körperschaften (Tb) oder Geographika (Tg) können fehlende Verknüpfungen auch maschinell behoben werden und die intellektuelle Arbeit entlasten. Dazu wird derzeit an der DNB an einem Vorschlagsystem gearbeitet, das Normdatenverknüpfungen für Strings in vorab definierten Feldern (z.B. Personen-Felder) vornimmt bzw. vorschlägt. Dabei werden maschinell Vorschläge für Verknüpfungen von Personen in Titeldaten mit bestehenden Tp-Sätzen, aber auch für neu zu erzeugende Tp-Datensätze generiert. Im letzteren Fall werden derzeit sogenannte Vorschlagsdatensätze (TX-Sätze) erzeugt, die nach intellektueller Prüfung zu Tp-Sätzen werden. Grundlage für die Erzeugung von Vorschlagdatensätzen ist das Vorhandensein einer Standardnummer wie etwa einer ORCID-ID, aber auch die Auswertung von Culturegraph-Werkbündeln oder der Open Access-Enginge BASE.

## Prozesse im Zusammenhang mit Datenimports

### 4.  Bulk-Import, Pre-Processing und Identifizieren von Entitäten (Entitätencodes)


## Prozesse im Zusammenhang mit der Qualitätssicherung / Sicherung der Metadatenqualität

### 5. Dubletten bereinigen 
Mit der Bereinigung von Dubletten verhält es sich ähnlich wie mit der Erschließung von Medien, dem Anlegen und Verknüpfen von Normdaten. Dubletten werden in der Regel dann händisch bearbeitet, wenn sie in der Erschließungsarbeit als Dubletten auffallen (work in progress). In der GND können Dubletten insbesondere dann gehäuft entstehen, wenn ein größeres Datenset von extern eingespielt wurde. Aus diesem Grund wird derzeit die sogenannte "GND-Toolbox" entwickelt ([Das Projekt "GND für Kulturdaten" (GND4C)](https://www.o-bib.de/article/view/5539/7880), S. 67ff.).  Diese soll die Anbindung neuer Datenquellen aus nicht-bibliothearischen Anwendungskontexten durch Bereitstellung von Schnittstellen unterstützen. Darüber hinaus soll die GND-Toolbox aber auch als Werkzeug zur Qualitätskontrolle der GND zur Verfügung stehen. Sowohl beim Pre-Processing von externen Datenbeständen als auch bei der Qualitätskontrolle kommen Match & Merge-Verfahren zum Einsatz. Im ersten Fall wird das externe Datenset gegen den Bestand der GND abgeglichen, um "Import-Kandidaten" zu identifizieren oder aber auszuschließen (siehe auch Prozess Nr. 4). Im zweiten Fall wird die GND gewissermaßen "gegen sich selbst gematched", um mögliche Dubletten zu identifizieren.
Ein regelmäßiges, automatisches Matching und Merging soll die Qualität und Konsistenz der GND-Datensätze künftig erhöhen und insofern auch die GND-Redakteur+innen entlasten, als die maschinell erkannten Dubletten unmittelbar als solche zur händischen Bearbeitung vorgeschlagen werden.

## Prozesse im Zusammenhang mit Anfragen an die GND (Anfragemanagement)

### 6. Anfragemanagement in der GND-Zentrale als Anlaufstelle für externe Partner+innen




