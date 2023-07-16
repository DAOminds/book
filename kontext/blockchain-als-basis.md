---
description: die Technologie hinter DAOs und ihre Bedeutung
---

# blockchain als basis

Ich komme nicht darum, hier kurz auf die einer DAO zugrunde liegenden Technologie einzugehen. Dabei habe ich nicht den Anspruch der Vollständigkeit- oder der vollen Tiefe. Vereinfacht ist eine Blockchain ein virtueller Computer, der auf einem Netzwerk physischer Computer läuft und starke, überprüfbare, spieltheoretische Garantien bietet, dass der von ihm ausgeführte Code weiterhin wie vorgesehen funktioniert. Blockchain-Systeme kombinieren dezentralisierte Netzwerke und kryptografische Funktionen auf neuartige Weise und schaffen einzigartige Eigenschaften, die die Unveränderlichkeit und Überprüfbarkeit von bestehenden Blockchain-Systemen unterstützen.

> « eine blockchain führt zur Dezentralisierung von Vertrauen und ermöglicht einen Wertestrom (Value Flow) ohne Intermediäre »

Das Ökosystem rund um Blockchains wächst unaufhörlich weiter. Um ein kurzen Überblick zu schaffen, nachfolgend eine Darstellung der verschiedenen Layer im Ökosystem. Ich fokussiere in diesem Teil nur auf den ersten Layer, das Fundament quasi.



<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption><p>blockchain layers</p></figcaption></figure>

* eine Blockchain ist keine Datenbank, wenn dann funktioniert die Blockchain wie ein Netzwerk mit replizierter Datenbanken
* eine Blockchain ist die Quelle der Wahrheit und ist in sich konsistent
* eine Blockchain ist kryptografisch sicher
* Blockchains führen zum Internet des Wertes
* Bitcoin ist eine Implementierung der Technologie Blockchain
* Bitcoin ≠ Blockchain

Eine Blockchain wird eingesetzt, wenn es keine einzige Partei gibt, der alle vertrauen. Und ja, zentralisierte Systeme sind schneller und meistens weniger komplex. Die Innovation einer Blockchain besteht darin, dass sie die Unveränderbarkeit und Sicherheit einer Aufzeichnung von Daten garantiert und Vertrauen schafft, ohne dass eine vertrauenswürdige dritte Partei erforderlich ist. Hier am Beispiel auf hoher Flughöhe am Beispiel einer Bitcoin-Transaktion.

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption><p>bitcoin transaction</p></figcaption></figure>

* Blockchain ist wenn dann eine Art gemeinsam genutzter Datenbank, die sich von einer typischen Datenbank durch die Art und Weise unterscheidet, wie sie Informationen speichert; Blockchains speichern Daten in Blöcken, die dann über Kryptografie miteinander verbunden werden.
* Wenn neue Daten eingehen, werden sie in einen Block integriert. Sobald der Block mit Daten gefüllt ist, wird er an den vorherigen Block angehängt, so dass die Daten in chronologischer Reihenfolge aneinandergereiht sind.
* In einer Blockchain können verschiedene Arten von Informationen gespeichert werden, aber die häufigste Verwendung war bisher die eines Hauptbuchs für Transaktionen.
* Im Fall von Bitcoin wird die Blockchain dezentralisiert eingesetzt, so dass keine einzelne Person oder Gruppe die Kontrolle hat, sondern alle Nutzer gemeinsam die Kontrolle behalten.
* Dezentralisierte Blockchains sind unveränderlich, was bedeutet, dass die eingegebenen Daten unumkehrbar sind. Für Bitcoin bedeutet dies, dass Transaktionen dauerhaft aufgezeichnet werden und für jeden einsehbar sind.

Eine der Besten Erklärungen der Blockchain-Prinzipien welche ich je gesehen habe, ist von Dan Boneh ([Blockchain Primitives: Cryptography and Consensus](../takeaways/empfehlung-videos/blockchain-fundamentals.md)), auch wenn teils technisch etwas anspruchsvoller.

### Sidechains

Eine Sidechain ist eine eigenständige Blockchain mit der zusätzlichen Eigenschaft, mit der Hauptblockchain interoperabel zu sein und Daten aus anderen Blockchains validieren zu können. Eine Sidechain kann mit einer oder mehreren anderen Chains kommunizieren und interagieren. Transaktionen sind die häufigste Interaktion mit einer Blockchain, die eine Kryptowährung unterstützt. Sidechains helfen die Skalierbarkeit von Blockchains zu erhöhen und angepasst an die Anforderungen die jeweils Beste Technologie einzusetzen. Sidechains bieten einen Mechanismus, um Funktionen auf einem Protokoll der ersten Schicht zu implementieren, ohne die Sicherheit oder Stabilität des Protokolls zu gefährden.

<figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption><p>sidechains</p></figcaption></figure>

Viele Blockchains, verwenden den Proof-of-Work als Konsens-Mechanismus und haben Kernfunktionen des Bitcoin-Protokolls übernommen. Daher haben sie viele der Einschränkungen des von Satoshi Nakamoto geschaffenen Codes geerbt. Dazu gehören ein begrenzter Durchsatz, hohe Latenzzeiten und eine begrenzte Skalierbarkeit. Sidechains stellen eine Möglichkeit dar, einige dieser technologischen Unzulänglichkeiten zu überwinden, aber sie öffnen nicht nur die Türen zu potenziellen technischen Entwicklungen, sondern berühren auch das Thema der Governance.

### Consens-Mechanismen

Es geht mit hier nicht darum, die Consens-Menchanismen von Blockchain im Detail zu erklären oder gar zu vergleichen. Nicht informierte tun die Krypto-Welt häufig ab mit dem Statement > „kann nichts sein, verschleudert Unmengen an Energie“. Aus meiner Sicht ist das lediglich eine natürliche Reaktion derer, welche nicht bereit sind eine Innovation genauer zu betrachten. Entsprechend liste ich nachfolgend ein paar Ansätze - welche auch angewandt werden - auf.

Führungskräfte, welche eine Blockchain-Technologie in Unternehmen einführen wollen, sollten gut über die verschiedenen Blockchain-Konsens-Mechanismen informiert sein. Obwohl sie ähnliche Ziele verfolgen, stellen verschiedene Blockchain-Konsens-Mechanismen den Konsens mit unterschiedlichen Ansätzen sicher. Einen einzigen zuverlässigen und für alle Anwendungsfälle genutzten Konsens-Mechanismus gibt es nicht. Die Mechanismen werden zudem laufend weiterentwickelt.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption><p>consens mechanisms</p></figcaption></figure>

**Proof of Work** \
Der Proof of Work (POW)-Prozess wird auch als Mining bezeichnet und die Miner werden als Nodes bezeichnet. Miner lösen komplizierte mathematische Rätsel, die eine hohe Rechenleistung erfordern. Zu diesem Zweck nutzen Miner verschiedene Mining-Methoden wie CPU-Mining, GPU-Mining, FPGA-Mining, Mining-Pools, ASIC-Mining und viele mehr. Nach dem Lösen von mathematischen Rätseln erhält ein Miner einen Block als Belohnung, wenn er als erster die Lösung gefunden hat. Ausserdem können die Rätsel nur durch Versuch und Irrtum gelöst werden. Daher benötigen die Schürfer immer mehr Rechenleistung, um die Lösungen schnell zu finden.

**Proof of Stake** \
Beim Proof of Stake (POS) wird nach dem Zufallsprinzip ermittelt, wer die Chance erhält, den nächsten Block zu erzeugen. Blockchain-Nutzer können ihre Token für eine bestimmte Zeit sperren, um Validator zu werden. Nachdem sie ein Validator geworden sind, können sie Blöcke produzieren. Validierer können auch auf der Grundlage des Designs der Blockchain ausgewählt werden. Im Allgemeinen hat der Nutzer, der den grössten Anteil oder die meisten Münzen über einen längeren Zeitraum besitzt, bessere Chancen, einen neuen Block zu erstellen.

**Delegierter Proof of Stake** \
Beim Delegated Proof of Stake-Verfahren können die Nutzer ihre Tokens einsetzen und für eine bestimmte Anzahl von Delegierten stimmen. Das Gewicht der Stimme eines Benutzers basiert auf seinem Einsatz. Wenn zum Beispiel ein Benutzer X" 20 Münzen für einen Delegierten einsetzt und ein anderer Benutzer Y" 2, dann hat die Stimme von X mehr Gewicht als die von Y. Der Delegierte, der die meisten Stimmen erhält, bekommt die Chance, neue Blöcke zu produzieren.

**Proof of Capacity** \
Bei der Methode des Kapazitätsnachweises werden die Lösungen komplexer mathematischer Rätsel in digitalen Speichern wie Festplatten gespeichert. Dieser gesamte Prozess wird als Plotten bezeichnet. Nachdem ein Speichermedium mit Lösungen für mathematische Rätsel gefüllt ist, können die Benutzer es zur Herstellung von Blöcken verwenden. Die Benutzer, die am schnellsten Lösungen finden, erhalten die Chance, einen neuen Block zu erstellen. Daher haben Benutzer mit der höchsten Speicherkapazität eine höhere Chance, einen neuen Block zu erzeugen.

**Proof of elapsed Time** \
Das Verfahren "Proof of Elapsed Time" (Nachweis der verstrichenen Zeit) entscheidet nach dem Zufallsprinzip und in fairer Weise über den Erzeuger eines neuen Blocks auf der Grundlage der von ihm verbrachten Wartezeit. Zu diesem Zweck sieht der Mechanismus eine zufällige Wartezeit für jeden Benutzer vor, und der Benutzer, dessen Wartezeit am frühesten endet, produziert einen neuen Block. Dieser Konsensmechanismus funktioniert nur, wenn das System sicherstellen kann, dass kein Benutzer mehrere Knoten betreiben kann und die Wartezeit wirklich zufällig ist.

**Proof of Identity** \
Der Identitätsnachweis vergleicht den privaten Schlüssel eines Benutzers mit einer autorisierten Identität. Im Grunde ist der Identitätsnachweis ein kryptografischer Beweis für den privaten Schlüssel eines Nutzers, der kryptografisch mit einer bestimmten Transaktion verbunden ist. Jeder identifizierte Nutzer eines Blockchain-Netzwerks kann einen Datenblock erstellen, der jedem im Netzwerk vorgelegt werden kann.

**Proof of Authority** \
Der Proof of Authority-Mechanismus ist eine modifizierte Version des Proof of Stake, bei dem es um die Identität der Validierer im Netzwerk geht. In diesem Szenario ist die Identität die Übereinstimmung zwischen der persönlichen Identifikation der Validierer und ihren offiziellen Dokumenten, die zur Überprüfung ihrer Identität dienen. Diese Validierer setzen ihren Ruf im Netz aufs Spiel. Beim Autoritätsnachweis sind die Knoten, die zu Validierern werden, die einzigen, die neue Blöcke erzeugen dürfen.

**Proof of Activity** \
Der Aktivitätsnachweis ist eine Kombination aus Proof of Work und Proof of Stake. Bei Proof of Activity versuchen die Miner, die Lösung eines Rätsels zu finden und ihre Belohnung einzufordern. Die Blöcke, die beim Proof of Activity-Mechanismus erstellt werden, sind jedoch einfache Vorlagen mit der Adresse der Mining-Belohnung und Header-Informationen. Die Header-Informationen werden dann verwendet, um eine zufällige Gruppe von Validierern für die Unterzeichnung eines Blocks auszuwählen. Die Validatoren mit grösseren Einsätzen haben eine grössere Chance, für die Unterzeichnung eines neuen Blocks ausgewählt zu werden.

### Das Blockchain Trilemma

Das Blockchain-Trilemma befasst sich mit den Herausforderungen, denen sich Entwickler bei der Entwicklung einer Blockchain stellen müssen, die skalierbar, dezentralisiert und sicher ist - ohne Kompromisse bei einer der Facetten einzugehen. Blockchains sind oft gezwungen, Kompromisse einzugehen, die verhindern, dass sie alle 3 Aspekte erfüllen:

* Dezentralisierung: Schaffung eines Blockchain-Systems, das nicht auf eine zentrale Kontrollstelle angewiesen ist
* Skalierbarkeit: die Fähigkeit eines Blockchain-Systems, eine immer grössere Anzahl von Transaktionen zu verarbeiten
* Sicherheit: die Fähigkeit des Blockchain-Systems, wie erwartet zu funktionieren und sich vor Angriffen, Fehlern und anderen unvorhergesehenen Problemen zu schützen

Während einige Entwickler glauben, dass die Blockchain-Datenstruktur selbst inhärente Beschränkungen aufweist, die eine Skalierung verhindern, sind viele Architekten, der Meinung, dass es möglich ist, ein Blockchain-Projekt zu entwickeln, das alle drei Ziele erreicht: skalierbar, dezentralisiert und sicher ist.

Erstens ist es wichtig zu beachten, dass das Trilemma nur ein Modell ist, um die verschiedenen Herausforderungen der Blockchain-Technologie zu konzeptualisieren. Es gibt kein Gesetz, das besagt, dass die drei Aspekte nicht erreicht werden können.

### Das Energie-Dilemma, welches keines ist?

Leider scheint momentan nur der Proof-of-Work Mechanismus und damit bspw. Bitcoin wirklich dezentralisiert zu sein. Oft wird argumentiert, dass das Bitcoin-Netzwerk Unmengen an Energie „verschleudert“. Zur Zeit benötigt das Bitcoin-Netzwerk um die 220 TWh (Terawattstunden) Energy pro Jahr. Um das in den Context zu bringen, ein paar Vergleiche:

* dies entspricht in etwa dem Bedarf z.B. von Schweden
* rund 10 mal soviel Energie, etwa 2’205 TWh, wird jedes Jahr produziert, aber kann und wird nicht genutzt, allein die USA [vernichtet jedes Jahr knapp 300 TWh](https://daominds.io/extwefenergyconsumtion) an Energie weil diese zwar produziert, aber nicht genutzt werden kann, alleine dies würde reichen um das Bitcoin-Netzwerk zu betreiben
* vergleichen wird die Marktkapitalisierung von Bitcoin und der S\&P Unternehmen und deren Energiebedarf, nutzt Bitcoin einen Bruchteil derer
* das globale Bankensystem verbraucht jährlich über 600 TWh an Energie
* die Goldbergbauindustrie hat im Jahr 2020 für die Produktion der gut 3’000 Tonnen an neuem Gold insgesamt 265 TWh an Energie verbraucht, die Stock to Flow Ratio bei Gold ist im übrigen bei rund 58, die von Bitcoin aktuell bei 53 und nach wird nach dem nächsten Bitcoin-Halving (2024) bei über 100 sein
* weniger als 1 % des globalen Stromverbrauchs von 27 PWh (Petawattstundenn) oder der 27’000 TWh werden vom Bitcoin Netzwerk genutzt, der globale Energiebedarf, Strom ist ein Teil davon beläuft sich auf rund 160 PWh (Bitcoin 0.14% hiervon)
* der Energieverbrauch des Bitcoin-Netzwerks entsprechen in etwa dem was global die „Lichterketten“ (Holiday Lights) oder die gespielten Computerspiele verbrauchen
* der derzeitige Energieverbrauch von Bitcoin entspricht in etwa dem der Kreuzfahrtindustrie
* weltweit gibt es aktuell rund 8 Mio. Elektroautos, dies entspricht einem Anteil von 0,6% der global rund 1,4 Mrd. Fahrzeugen und einem Energiekonsum von 90 TWh. Was wäre wenn rund 10% der Autos global Elektroautos wären?

Die Bitcoin-Miner gehen dort hin und nutzen die Energy welche günstig ist, d.h. erneuerbare Energien spielen eine wichtige Rolle bei der Erzeugung neuer Bitcoin und dem Betrieb des Bitcoin-Netzwerks, und die Miner haben einen wirtschaftlichen Anreiz, dies beizubehalten und nach billigen, sonst möglicherweise unzugänglichen Energiequellen zu suchen oder verwenden überschüssige Energie, einige Beispiel:

* verschieden Schätzungen gehen davon aus, dass zwischen 40 - 73% der durch das Bitcoin geuzten Energy erneuerbar ist, mehr als der weltweite durchschnittlichen Anteil erneuerbarer Energien am Energiemix, der sich auf etwa 28 % beläuft
* die Argumentation über den Energieverbrauch pro Transaktionen ist irreführend, [die Anzahl der Transaktionen skaliert nicht mit der nötigen Energy für das Mining im Bitcoin Netzwerk](https://daominds.io/extenergyconsumedbybitcoin). Einerseits entwickelt sich die Hash-Rate des Netzwerks nicht parallel zum Energieverbrauch, weil die Miner grundsätzlich effektiver werden. Zudem werden sogenannte Layer2 Lösungen wie das Lightning-Netzwerk eingesetzt, um nicht alle Transaktionen On-Chain bzw. auf der Blockchain abzuwickeln
* [Wasserkraftwerke nutzen die Energy für das Bitcoin-Mining](https://daominds.io/exthydrolecticpowerforbitcoin), weil dies für sie rentabler ist, hier scheint der zu tiefe Energiepreis ein Problem zu sein
* jedes Jahr werden 150 Milliarden Kubikmeter an Gas mit Gas Flaring eliminiert, hier setzen [Miner darauf diese Energy zu nutzen](https://daominds.io/extflaredgasforbitcoin), das Unternehmen Crusoe Energy Systems hat mit dem Produkt Digital Flare Mitigation eine Lösung für Deep-Learning, Bitcoin-Mining und anderer rechenintensiven Use-Cases im Angebot. Medienberichten zufolge führt ExxonMobil ein Pilotprojekt durch, bei dem es industrielle Gaslecks als Energie für Bitcoin-Farmen verkauft.
* El Salvador bspw. nutzt [Abwärme eines Vulkans um Bitcoin zu minen](https://daominds.io/extelsalvadorminebyvulkan)
* in Skandinavischen Ländern wird viel mit Strom geheizt, würde die nötige Wärme indirekt über Bitcoin-Miner generiert, würde dies dem aktuellen Bedarf des gesamten Bitcoin-Nerzwerk entsprechen

Natürlich ist Bitcoin ein Energie-Nutzer. Wenn ich den Mehrwert von Bitcoin nicht sehe, sinkt natürlich die Toleranz bezüglich der verbrauchten Energie. Ich glaube es gibt definitiv mehrere Perspektiven. Persönlich würde ich so weit gehen, dass Bitcoin eine Entwicklung in Richtung von erneuerbaren Energien sogar fördert. Was deine Perspektive ist, überlasse natürlich dir.  Wichtig an dieser Stelle, sämtliche Blockchain welche nicht einen Proof-of-Work Mechanismus einsetzen, benötigen eben auch nicht dermassen Energie. DAOs setzen in aller Regel auf Technologien, welche mit Bitcoin nichts zu tun haben.   Eine Liste der in Bezug auf DAO’s relevanten Blockchains findest du unter \[DAOMinds DAO Technology].
