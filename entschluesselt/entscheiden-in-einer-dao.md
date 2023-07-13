---
description: wie Transparenz und Effizienz gewährleistet wird
---

# entscheiden in einer dao

Blockchain-Governance kann sich auf zwei Konzepte beziehen: entweder die Governance eines Blockchain-Systems (autonome) oder die Nutzung eines Blockchain Systems zur Steuerung einer externen Organisation oder eines Prozesses (nicht autonom). In diesem Kapitel werden ausschliesslich die „nicht autonomen“ Entscheide betrachtet, welche durch On-Chain-Regeln definiert werden können. Eine DAO ist für mich ein Beispiel für die Grenzen der On-Chain Governance.

Die Governance in DAOs besteht effektiv aus zwei Ebenen:

* einer sozialen Ebene, z. B. die Diskussionen in [Discord](https://daominds.io/extdiscord) zur Unterstützung eines Förderantrags
* einer Abstimmung auf der Grundlage des Token-Besitzes mit [Snapshot](https://daominds.io/extsnapshot) oder [WithTally](https://daominds.io/extwithtally) oder ähnlich

DAO-Governance-Frameworks ermöglichen es, Änderungen an verschiedenen Aspekten des Projekts vorzuschlagen, zu diskutieren und umzusetzen, ohne sich auf ein Kernteam oder eine zentrale Instanz zu verlassen oder diese zu benötigen.

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption><p>decentralized autonomous corporate governance</p></figcaption></figure>

Dezentralisierte Entscheidungsfindung ist schwierig. Bis heute gibt es keine klaren Best Practices für die Governance und es gibt noch viel zu lernen. Bitcoin hat eine wirklich dezentralisierte Governance-Struktur (es gibt keinen Gründer, auf den die Gemeinschaft schaut, und es ist sehr schwer, Änderungen am Protokoll vorzunehmen), was gut funktioniert, wenn man versucht, ein Protokoll zu sein, das als Wertaufbewahrungsmittel dient und nicht viel iterieren muss, aber es funktioniert nicht gut für die meisten Technologieprojekte in der Frühphase, die oft und schnell iterieren müssen. Meiner Meinung nach ist eine gewisse Zentralisierung der Entscheidungsfindung in den ersten Tagen eines Projekts generell notwendig. Die besten Projekte werden wahrscheinlich so konzipiert sein, dass sie langfristig in allen Bereichen der Organisation dezentralisiert sind, aber nicht unbedingt von Anfang an.

| <p><strong>Ausführung &#x26;</strong><br><strong>Entscheidungsfindung</strong></p> | <p><strong>zentralisierte</strong></p><p><strong>Entscheidungsfindung</strong></p> | <p><strong>dezentrale</strong></p><p><strong>Entscheidungsfindung</strong></p> |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| <p>nicht autonome</p><p>zentralisierte Ausführung</p>                              | <p>Traditionelles<br>Unternehmen</p>                                               | Kooperation                                                                    |
| <p>nicht autonome</p><p>aggregierte Ausführung</p>                                 | Kult                                                                               | Community                                                                      |
| <p>nicht autonome</p><p>gemeinsame Ausführung</p>                                  | n/a                                                                                | n/a                                                                            |
| <p>autonome</p><p>zentralisierte Ausführung</p>                                    | <p>autokratische<br>Nationen - Staat</p>                                           | <p>repräsentativer demokratischer<br>Nationalstaat</p>                         |
| <p>autonome</p><p>aggregierte Ausführung</p>                                       | Autonomer Kult                                                                     | aufstrebende DAO                                                               |
| <p>autonome</p><p>gemeinsame Ausführung</p>                                        | <p>sozial/kulturell<br>gefangener DAO</p>                                          | DAO                                                                            |

### Signal Voting

Beim Signal Voting signieren Token-Inhaber ihre Stimmen mit dem öffentlich-privaten Schlüsselpaar. Auf diese Weise kann jeder, der eine Liste der signierten Stimmen hat, die Signatur überprüfen, sehen, dass er Token auf der Blockchain hat, und die Stimmen zusammenzählen. Normalerweise werden die Stimmen bei der Signalabstimmung nach Token gewichtet, d. h. die Wähler erhalten eine Stimme pro Token. Die Signalabstimmung erfolgt nicht auf der Blockchain direkt, was bedeutet, dass diese kostenlos ist. Das bedeutet aber auch, dass die Abstimmung selbst keinen Einfluss auf die Blockchain hat. Projekte brauchen einen anderen Baustein, um das Ergebnis einer Abstimmung zu übernehmen und die Dinge auf der Blockchain zu ändern. Wichtig ist, dass das Signieren von Nachrichten ausserhalb der Blockchain nicht garantiert, dass alle anderen die Nachricht sehen können. Die Signalabstimmung hängt von einem Server wie [Snapshot](https://daominds.io/extsnapshot) oder einem Peer-to-Peer-Broadcast-Netzwerk wie libp2p ab, um Abstimmungen zu übertragen.

### On-Chain Voting

Eine On-Chain-Abstimmung ist das, wonach es klingt. Token-Besitzer können im Verhältnis zu ihrem Token-Guthaben Vorschläge erstellen und darüber abstimmen. Die Stimmen werden auf die Blockchain übertragen, so dass ein Governance-Smart-Contract die Stimmen zusammenzählen und bestimmen kann, welche Vorschläge angenommen werden. Governor Alpha von [Compound](https://daominds.io/extcompound) gilt für viele Projekten als sinnvoller Ansatz. Die On-Chain-Abstimmung kostet Geld. Die Hypothese ist, das wenn man für eine Simse bezahlt, wird das System sicherer und dezentraler. Die Governance ist in diesem Fall nicht auf eine dritte Partei angewiesen, um die Stimmen zu übermitteln, da die Verfügbarkeit auf der Blockchain selbst sichergestellt ist.

### Multisig Admin

Multisigs gab es schon, bevor es Blockchains überhaupt gab. Bei einer Multisig teilt sich eine feste Anzahl von Adressen die Verwaltungsbefugnis, ähnlich wie die Regeln in einem Handelsregister. Eine Teilmenge von ihnen - z. B. 3 von 5, alle 4 von 4 oder sogar 1 von 2 - hat die Befugnis, Entscheide zu fällen. Das Gnosis-Team hat Safe entwickelt, einen weit verbreiteten und erprobten Smart Contract, der Multisigs beliebiger Grösse auf Ethereum implementiert. Dieser Vertrag wird häufig für die Verwaltung von Protokollverträgen und On-Chain-Schatzkammern verwendet.

|                               | Signal Voting        | On-chain Voting                    | Multisig Admin                       |
| ----------------------------- | -------------------- | ---------------------------------- | ------------------------------------ |
| Offen für                     | jeden Token Besitzer | jeden Token Besitzer               | geschlossener Kreis von Admins       |
| Stimmgewicht                  | Token-abhängig       | Token-abhängig                     | eine Stimme pro Admin                |
| Kosten                        | Kostenlos            | Wählende zahlen Transaktionskosten | Admins zahlen Transaktionskosten     |
| Soziale Skalierbarkeit        | jeder kann abstimmen | jeder kann abstimmen               | Abstimmungen in einem Unterausschuss |
| Datenverfügbarkeit            | auf einer Plattform  | auf der Blockchain                 | auf der Blockchain                   |
| Ausführung auf der Blockchain | nicht direkt         | ja                                 | ja                                   |
| Geschwindigkeit               | Tage                 | Tage                               | Sofort                               |
| Stärke                        | Kostenlos            | Sicher                             | Schnell                              |

### Kombination der Ansätze

#### **Signal Voting + Admin-Multisig = Snapshot** 

Vielleicht kennen Sie Snapshot, ein beliebtes Tool für Projekte, um ihre Verwaltung zu steuern. Da das Tool auf Signalabstimmung basiert, kann jeder Token-Inhaber kostenlos auf Snapshot abstimmen. Wie erwähnt, wird bei der Signalabstimmung nichts auf der Blockchain ausgeführt. Normalerweise hängen Snapshot-Abstimmungen von einem Admin-Multisig ab, um den Willen der Wähler auf der Blockchain genau und prompt auszuführen. Kürzlich kündigte Snapshot an, dass sie das [reality.eth Orakel](https://daominds.io/extrealityoracle) verwenden werden, um die Vorschläge auf der Kette auszuführen.

#### **Signal Voting + On-Chain-Abstimmung = Lebenszyklus von der Idee zum Vorschlag** 

Radicle ist eines der vielen Projekte, die einen Vorschlagslebenszyklus mit Signalabstimmung und On-Chain-Abstimmung verwenden. Im Fall von Radicle wird Snapshot als unverbindlicher Temperatur-Check verwendet, um zu sehen, welche Ideen Unterstützung zu haben scheinen. Sobald eine Idee den Temperatur-Check bestanden hat, können die Mitglieder der Radicle-Community die Idee in ihren Foren zu einem formellen Vorschlag verfeinern. Schliesslich reichen sie den Vorschlag als ausführbaren Code zur Abstimmung auf Radicle Governor Alpha ein. Dieser Lebenszyklus nutzt den kostenlosen Schritt - die Signalabstimmung - um es einfach zu machen, neue Ideen einzubringen, und nutzt den teuren, aber sicheren Schritt - die On-Chain-Abstimmung - um den Vertrag und die Kasse sicher zu halten.

#### **On-Chain-Abstimmung + Admin-Multisig = Übertragung von Befugnissen an einen Ausschuss**

Sowohl Uniswap als auch Compound haben vor kurzem On-Chain-Abstimmungen durchgeführt, um Ausgabenbefugnisse an die Multisigs zu delegieren. Uniswap schlug das Uniswap-Zuschussprogramm (Grants Program) vor, und Compound folgte kurz darauf mit dem Compound-Zuschussprogramm. Nach ihrer Verabschiedung finanzierten diese Vorschläge jeweils eine Multisig, deren Aufgabe es ist, die Arbeit im Ökosystem des jeweiligen Projekts zu finanzieren.

Viele Ideen und Ansätze befinden sich aktuell in der Konzept- oder Umsetzungsphase. Es ist davon auszugehen, dass in dieser Thematik noch vieles passieren wird.

#### Tools in Web

* [Tally](https://daominds.io/extwithtally) empowers user owned governance through real time research and analysis, governance tooling, and evergreen educational content
* [Snapshot](https://daominds.io/extsnapshot) a decentralized voting system.
* [Boardroom Insights](https://daominds.io/boardroom) a ressource for distributed organizations an their governance
