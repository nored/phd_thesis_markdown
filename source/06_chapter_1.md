
# Einleitung

## Motivation

In den letzten Jahren war eine Verschiebung vom Supercomputer-Computing hin zum Cloud-Computing zu beobachten. Infolgedessen hat sich die horizontale Skalierbarkeit erhöht, aber auch die Komplexität ist gewachsen. In großen verteilten Systemen reicht es nicht mehr aus, das Caching von hoch frequentierten Daten in einzelne Anwendungen oder Systeme einzubetten. Da zukünftige Datenanfragen aus der horizontal verteilten Cloud aus allen Richtungen kommen können und keinem Determinismus unterliegen, bedarf es eines Objektcaches.
 
Ein Objekt-Cache ist eine dedizierte Anwendung, die für die Speicherung von teuren Berechnungsergebnissen verantwortlich ist. Zum Beispiel kann in einer Anwendung zur Textanalyse ein Wort besonders viele Querreferenzen besitzen. Die Berechnung und Indexierung dieser Referenzen hat bereits bei der Erstellung einiges an Rechenzeit und Leistung gekostet. Eine erneute Referenzierung bei jeder Anfrage würde nicht nur unnötig Last erzeugen, es könnte große Analysen zeitmäßig schlichtweg unmöglich machen. Stattdessen wird die Berechnung nur ein einziges mal ausgeführt und das Ergebnis im Objektcache gespeichert. Nachfolgende Anfragen rufen die Ergebnisse aus dem Cache ab und vermeiden die Kosten der Berechnung.  

## Aufgabenstellung

Das Hauptaugenmerk dieser Arbeit liegt nun in den Datenstrukturen, mit denen diese Objektcaches umgesetzt werden und deren Einfluss auf die Performanz in modernen verteilten Systemen. Dazu wird in dieser Arbeit die In-Memory-Datenbank Redis wie beschrieben genutzt um zu evaluieren, ob und wie sich die verfügbaren Strukturen in Diskrepanz zur Performanz auf das Caching auswirken. Durch das Aggregieren großer Mengen einfacher zu cachender Daten, soll durch das sukzessive Verändern der Datenstruktur selbiger herausgefunden werden, wie sich im Verhältnis dazu die Performanz in Form der Antwortzeit auf eine möglichst hohe Anfrage-Dichte ändert und ob es dabei eine Relation zur Speicherbreite der jeweiligen Struktur gibt.
 
## Abgrenzung

## Aufbau der Arbeit

