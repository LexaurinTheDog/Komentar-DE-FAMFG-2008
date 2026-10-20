# Quellen und Reproduzierbarkeit

Bearbeitungsstichtag und tatsächlicher Abruf: **19. Oktober 2026**. Die Quellen wurden lokal gesichert; das Original-Intake wurde nicht verändert.

Erneute Quellenvorprüfung: **20. Oktober 2026**, bei unverändertem Bearbeitungsstichtag. [Heutige ZIP-Lieferung](sources/famfg-2026-10-20.zip), [heutiges XML](sources/famfg-2026-10-20.xml), [HTML-Index](sources/famfg-index-2026-10-20.html), [Gesamt-HTML](sources/famfg-full-2026-10-20.html) und [Aktualitätendienst](sources/current-service-2026-10-20.html) sind mit tatsächlichem HTTP-Ergebnis und Hash im Verifikationsprotokoll erfasst. Die FamFG-Dateien sind gegenüber dem 19. Oktober bytegleich. Alle drei einschlägigen Änderungsgesetz-PDFs wurden erneut erfolgreich geladen und sind ebenfalls bytegleich. Artikel 4 Nummer 4 der Nr. 192 ändert zusätzlich die Verweisung in § 113 Absatz 1; auch diese Änderung ist im ausgewählten Text enthalten.

Der [Vorprüfungsbericht](preflight-result.json) verbindet die tatsächlichen Inkrafttretensregeln mit konkreten Textprüfungen. Die [ergänzende Verkündungsprüfung](sources/recent-enactments-check.json) sichert sieben vollständig durchsuchte amtliche Gesetzes-PDFs aus dem neueren Aktualitätendienst: Nr. 275, 276, 285, 286, 289, 293 und 304. Es ergab sich kein Fund für FamFG, Familiensachen oder freiwillige Gerichtsbarkeit. Die Auswahl schließt vorsorglich späte Septembergesetze vor dem Intake ein; Verordnungen und Berichtigungen wurden anhand ihrer Titel gesichtet. Dies ist keine lückenlose historische Prüfung aller Verkündungen.

Der Vollständigkeitsbericht enthält nun ein Einzelinventar sämtlicher XML-Normelemente sowie Zeichenvergleiche aller Quellenhinweise und Gliederungen. Gesetzeskopf und Inhaltsübersicht enthalten keine übergangene operative Eingangsformel. Die Hinweise zur Entstehung als Artikel 1 des FGG-RG und zum ursprünglichen Inkrafttreten bleiben in der kanonischen Transkription erhalten. Der Parser bricht bei bislang unbekannten Normtypen oder doppelten Paragraphenkennungen ab. Es wurden keine neuen Kommentare verfasst und keine vorhandenen Kommentare verändert.

## Gesetzestext

- [Gesetze im Internet, FamFG](https://www.gesetze-im-internet.de/famfg/): [Index-Snapshot](sources/famfg-index.html), [vollständiges HTML](sources/famfg-full.html).
- [XML-ZIP](https://www.gesetze-im-internet.de/famfg/xml.zip): [gesicherte ZIP-Datei](sources/famfg-2026-10-19.zip), [entpacktes XML](sources/famfg.xml). Erwartete Wurzel `dokumente`, Kennung `BJNR258700008`, Abkürzung FamFG; ZIP geöffnet, XML tatsächlich geparst. Kein HTML-Ersatz als XML akzeptiert.
- [Aktualitätendienst](https://www.gesetze-im-internet.de/aktuDienst.html): [Snapshot](sources/current-service.html), ergänzende Aktualitätskontrolle am Stichtag.
- [Kanonische Texttranskription](sources/famfg-canonical.md), [Intake-Kopie](sources/intake-2026-10-01.md), [Änderungskarte](sources/change-map.json). Die Transkription wird durch `_parse.py` aus dem XML erzeugt; die Zeichenfolge wird unabhängig unter Ausblendung bloßer Leerraumformatierung gegengeprüft.

Der amtliche Inhaltsüberblick und die eigentlichen Normmetadaten enthalten unabhängig voneinander dieselben 529 Paragraphenkennungen. 68 echte Gliederungselemente, Gesetzeskopf und Inhaltsübersicht ergeben zusammen mit den Paragraphen 599 XML-Normen. Die Angabe 598 aus dem Intake war deshalb keine verlässliche Paragraphenzahl. Operative Anlagen außerhalb dieser Einheiten sind im XML nicht vorhanden. Schluss- und Übergangsbestimmungen §§ 486–493 gehören zur erfassten Liste. Entfallene Gesamt- und Teilvorschriften werden nicht als Lücken versteckt.

Die sechs rohen Intake-Differenzen betreffen Quellenhinweise bei §§ 14a und 162 und die explizite Wiedergabe der in Überschriften bezeichneten leeren Einheiten §§ 190, 230, 289 und 364. Sie belegen keine sechs neu erlassenen Vorschriften. Die amtliche Standdokumentation wurde aktualisiert; der erfasste materielle Paragraphenwortlaut stimmt nach Bereinigung dieser Darstellungsfragen mit dem Intake überein.

## Inkrafttreten tatsächlich kontrolliert

- [BGBl. 2026 I Nr. 152](https://www.recht.bund.de/bgbl/1/2026/152/VO.html): [Original-PDF](sources/bgbl-152.pdf), [Textextraktion](sources/bgbl-152.txt). Artikel 6 fügt § 95 Absatz 5 an; Artikel 18 Absatz 1 bestimmt den 1. Oktober 2026.
- [BGBl. 2026 I Nr. 192](https://www.recht.bund.de/bgbl/1/2026/192/VO.html): [Original-PDF](sources/bgbl-192.pdf), [Textextraktion](sources/bgbl-192.txt). Artikel 4 betrifft § 41a und § 46 Absatz 2; maßgebliches Inkrafttreten nach Artikel 20 Absatz 1 am 1. Oktober 2026.
- [BGBl. 2026 I Nr. 198](https://www.recht.bund.de/bgbl/1/2026/198/VO.html): [Original-PDF](sources/bgbl-198.pdf), [Textextraktion](sources/bgbl-198.txt). Artikel 10 Absatz 1 Nummer 2 setzt Artikel 4 Nummer 8 am Tag nach Verkündung, somit am 10. Juli 2026, in Kraft. Das betrifft § 214 Absatz 2 Satz 3. Die übrigen hier betroffenen FamFG-Erweiterungen gelten nach Artikel 10 Absatz 2 erst am 1. Juli 2027. Neue §§ 94a–94d, § 167c und § 216b werden deshalb nicht als gegenwärtige Lücken behandelt.

Die PDF-Abrufe lieferten HTTP 200 und tatsächliche `%PDF-`-Dateien; eine bloße HTML-Fehlerseite wurde nicht als PDF übernommen. Die Auswertung der Inkrafttretensartikel erfolgte aus den vollständig gesicherten Originaldateien. Nicht behauptet wird eine nochmalige Prüfung jeder historischen Änderung seit 2008.

## Rechtsprechung und Suche

Die [Fallkartenübersicht](cases/README.md) enthält vier vollständig gelesene amtliche Entscheidungen; zwei davon wurden in der begrenzten Zweitprüfung ergänzt und mit ihren jeweiligen Verwendungsgrenzen dokumentiert. Der lokale nationale Rechtsprechungsbestand wurde nach konkreten Aktenzeichen abgefragt. Die offiziellen RII-ZIP-Dateien wurden neu abgerufen und als XML validiert. Die Karten trennen Tatbestand, Vorinstanz, gerichtliche Aussagen und Anwendungsgrenzen.

[Suchprotokoll](sources/search-log.json), [Firecrawl-Suchergebnis](sources/firecrawl-current-search.json). Der BGH-HTML-Abruf zu XII ZB 114/21 lieferte eine Startseite statt der Entscheidung und wird ausdrücklich als verworfen geführt. Der amtliche RII-Volltext ersetzt diesen ungeeigneten Abruf. Die gesicherte Entscheidung XII ZB 601/15 wurde nicht vollständig ausgewertet und nicht zur Autorität erhoben. Keine vollständige Rechtsprechungsauswertung für das gesamte FamFG und keine Behauptung, bei nicht zitierten Einheiten existiere keine relevante Entscheidung.

## Nachweise und Grenzen

[Verifikationsprotokoll](sources/verification.json) mit tatsächlichen URLs, Zeitstempeln, HTTP-Ergebnissen, Formatprüfungen und SHA-256; [Quellenmanifest](source-manifest.json) mit lokalen Dateiprüfsummen; [Vollständigkeitsbericht](completeness-report.json); [technischer Audit](technical-audit.json); [strenge Gesamtvalidierung](validation.json); [regulärer Buildversuch](build-result.json).

Die Ausgabe ist unvollständig: 193 kommentierte und 336 noch nicht kommentierte Einheiten. Die unabhängige zweite Sachprüfung ist bislang auf die 20 Einheiten §§ 1–18 einschließlich §§ 14a und 14b beschränkt. Weitere Einzelheiten in [REVIEW](REVIEW.md). Rechte am amtlichen Wortlaut werden nicht durch die Kommentarlizenz beansprucht; [amtlich geprüfter § 5 UrhG](sources/urhg-5.html).

## Ergänzende Quellen der begrenzten Zweitprüfung

Am 20. Oktober 2026 wurden [FamFG-ZIP](https://www.gesetze-im-internet.de/famfg/xml.zip), [Inhaltsübersicht](https://www.gesetze-im-internet.de/famfg/) und [ZPO-ZIP](https://www.gesetze-im-internet.de/zpo/xml.zip) tatsächlich mit HTTP 200 abgerufen. Lokale Belege: [FamFG-XML](sources/review-p1-p18-famfg.xml), [Index](sources/review-p1-p18-index.html), [ZPO-XML](sources/review-p1-p18-zpo.xml). Identität, Format und Prüfsummen stehen im Verifikationsprotokoll. Die FamFG-Datei ist bytegleich mit der Fassung vom Bearbeitungsbeginn; der Bearbeitungsstichtag bleibt der 19. Oktober 2026. Die ZPO wurde gezielt für die in §§ 9, 11, 13, 14, 16 und 17 behandelten Verweisungen geprüft, nicht als eigenständig vollständig kommentiertes Gesetz. § 233 Satz 2 ZPO enthält heute bereits die Vermutung bei Belehrungsmängeln.

Die zwei neuen [Fallkarten](cases/README.md) belegen die selektive Recherche zu §§ 14b und 17. Die lokalen nationalen Fundstellen wurden mit frisch abgerufenen offiziellen ZIP/XML-Volltexten abgeglichen. Firecrawl war authentifiziert, meldete jedoch kein verfügbares Guthaben; deshalb wurden die amtlichen Rohdaten unmittelbar abgerufen. [Suchprotokoll](sources/search-log.json), [Prüfungsergebnis](review-result.json).


## Begrenzter Prüfungsnachtrag §§ 19–36a vom 20. Oktober 2026

Der neue [FamFG-XML-Snapshot](sources/review-p19-p36a-famfg.xml) ist mit der amtlichen Grundlage vom 19. Oktober bytegleich. Die [ZPO-XML](sources/review-p19-p36a-zpo.xml) dient dem tatsächlichen Abgleich der verwiesenen Beweis-, Termin-, Vergleichs- und Zwangsmittelregeln. Alle Abrufe einschließlich neuer Rechtsprechungsbelege stehen mit HTTP-Resultat, Datum, Formatprüfung und SHA-256 in [verification.json](sources/verification.json); Suchwege und Grenzen in [search-log.json](sources/search-log.json). Das [aktuelle Einzelprotokoll](review-result.json) erfasst genau 20 Einheiten, die [erste Charge](review-p1-p18-result.json) bleibt getrennt erhalten. Die neue bayerische Fallquelle wird ausschließlich anhand des gerichtlichen Tenors und der vollständigen Gründe ausgewertet; redaktionelle Leitsätze des Webseitenbelegs sind keine Kommentierungsgrundlage.


## Quellen der begrenzten Prüfung §§ 37–55 vom 20. Oktober 2026

Frischer [FamFG-XML-Beleg](sources/review-p37-p55-famfg.xml) und [HTML-Index](sources/review-p37-p55-index.html), jeweils HTTP 200, stimmen mit der früheren Textlieferung überein. Version und Inkraftsetzung: [BGBl. 2026 I Nr. 192](sources/bgbl-192.pdf), Artikel 4 und 20; ausführliche [Vorprüfung](preflight-result.json). [Verifikationsprotokoll](sources/verification.json) enthält URL, UTC-Zeitstempel, Formatprüfung und SHA-256.

Neu ausgewertet: [BGH XII ZB 674/14](cases/BGH-XII-ZB-674-14.md), amtlicher vollständiger Tenor und Rn. 1–37. Gesichert sind [XML](sources/review-p47-XII-ZB-674-14.xml), [lesbare Gründe](sources/review-p47-674-14-gruende.txt) und [lokaler Korpusbeleg](sources/review-p47-local-KORE301152015.md). Nur die historisch begrenzte Aussage zu § 47 wird genutzt. Der ebenfalls gesicherte Fall XII ZB 89/15 wurde nach Identitäts-/Tenorprüfung ausgeschieden; keine vollständige Lektüre oder Verwendung behauptet. Einzelheiten und fehlgeschlagene Webzugriffe stehen im [Suchprotokoll](sources/search-log.json). Der amtliche ZPO-Beleg aus der vorherigen Charge wurde für § 573 erneut gelesen.
