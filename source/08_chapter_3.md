
# Vergleichbare Arbeiten

## 1

## 2

## 3

<!--
## Erwartetes Ergebnis

Da Redis kein reiner Key-Value Store ist, kann es zu großen Unterschieden in der Performanz der einzeln genutzten Datenstruktur kommen. Zwar werden einzelne Datensätze streng nach dem Prinzip eines Key-Value Stores abgespeichert, die interne Umsetzung variiert aber stark. So unterstützt Redis die Speicherung zum Beispiel in reinen binary-safe Strings ohne weitere Indexierung, Sortierung oder Score Wert. Es ist anzunehmen, dass eine derartige Struktur eine sehr gute Performanz bei der Verarbeitung der Daten während der Aggregation erreicht. Bezweifelt werden kann jedoch, dass so gespeicherte Daten in der Masse besonders schnell durch redis gefunden werden. Somit sollte sich für diese Datenstruktur eine sehr schlechte Performanz bei der Antwortzeit einer Anfrage ergeben und das, obwohl es sich dabei um die kleinst mögliche Struktur handelt, die Redis zu bieten hat. Weiterhin ist zu erwarten, dass sogenannte "sorted Sets", bei denen es sich um Listen handelt die mit einem Score Wert versehen wurden bei bestimmten Anfragen, nämlich solchen, bei dem die Macht der Score Zahl ausgespielt werden, kann eine sehr gute Performanz abliefern ungleich zu ihrer Größe im Vergleich zu reinen Strings. Allgemein wird erwartet, dass sich alle in Redis möglichen Strukturen relativ zur O'Notation jener Datenstruktur verhalten nach deren Vorbild sie implementiert wurden. Allgemein auszuschließen ist, dass sich durch das Ändern der Datenstruktur eine Änderung der Antwortzeit ergibt, welche sich fest in Relation zur Speichernutzung der jeweiligen Struktur verhält. Da sich die Speicherbreite je Struktur stark unterscheidet könnte eine ebenso stark schwankende Performanz durch selbiges bedingt erwartet werden. Durch den Vorteil einiger Datenstrukturen in der Suchgeschwindigkeit gegenüber anderen sollte das gesamte Performanz-Bild jedoch in Diskrepanz zum Speicherverbrauch durch diesen Faktor dominiert werden [@TICP S.12-22].     
--> 
