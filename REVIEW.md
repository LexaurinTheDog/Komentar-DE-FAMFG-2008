# Eigenkontrolle und ausstehende Bearbeitung

**Keine unabhängige Zweitprüfung. Kein externes fachliches Freigabeurteil.** Dieses Protokoll dokumentiert die Eigenkontrolle des noch unvollständigen Arbeitsentwurfs vom 19. Oktober 2026.

## Vorhandener Bestand

§§ 1–168g sind mit 193 vorschriftenspezifischen Kommentierungen vorhanden. Der Abschnitt Kindschaftssachen endet damit einschließlich der eingefügten Regeln zur Vormundschaft und standesamtlichen Mitteilung. Der gesamte amtliche Normbestand enthält 529 Paragrapheneinheiten. Die 336 Einheiten ab § 169 sind noch nicht kommentiert; ihre vollständigen Kennungen stehen in `completeness-report.json`.

Geprüft wurden die im bearbeiteten Bereich verwendeten Gesetzespassagen beim Schreiben, die Zuordnung von eigenständiger Beteiligung und bloßer Anhörung, die Sonderweiche des § 113, Unterschiede zwischen Einlegung und Begründung von Rechtsmitteln, die Grenzen der Kindesanhörung und die zum Stichtag erst künftig wirksamen Gewaltschutzänderungen. Zwei verwendete BGH-Volltexte wurden einschließlich ihrer jeweiligen Grenzen gelesen. Dies ist keine Aussage, dass sämtliche denkbaren Auslegungsstreitigkeiten erschöpfend behandelt seien.

## Technische Kontrollen

Der Parser ist reproduzierbar. Vollständige amtliche Inhaltsübersicht und Normmetadaten werden getrennt ausgelesen und stimmen mit den extrahierten 529 Kennungen ohne fehlende oder doppelte Einheit überein. Alle Textzeichen stimmen unter Ausblendung bloßer Leerraumformatierung mit den jeweiligen XML-Content-Blöcken beziehungsweise ausdrücklich leeren Überschriftseinheiten überein. Absatz- und Untergliederung werden in der Lesefassung bewahrt.

Die Ausgangs- und Aktualitätsquellen sowie drei relevante Verkündungsakte sind gesichert. Formate und Hashes wurden geprüft. Quellenmetadaten und Wortlautänderungen werden in der Änderungskarte nicht gleichgesetzt. Die technische Prüfung erfasst lokale Links, vorhandene Kommentierungsblöcke, Längen, exakte Wiederholung längerer Absätze und auffällig ähnliche Wortbestände. Kein solcher Test beweist sachliche Richtigkeit oder ausreichende Kommentierungstiefe.

## Offene materielle Arbeit

Der vollständige Kommentar ab § 169, darunter Abstammung, Adoption, weitere Familiensachen, Betreuung und Unterbringung, Nachlass und Teilung, Register, Freiheitsentziehung, Aufgebot und Schlussrecht, fehlt noch. Die Wortlautdatei ist hierfür vorhanden; sie ist kein Ersatz für originäre Erläuterungen.

Die Rechtsprechungsrecherche bleibt selektiv und muss für die noch fehlenden Sachgebiete fortgesetzt werden. Ein vorhandener, nicht ausgewerteter Download darf nicht ohne tatsächliche Lektüre als geprüft gelten. Auch der vorhandene Kommentar benötigt eine frische unabhängige zweite Prüfung auf Auslegung, Verweise, Anwendungsgrenzen und Aktualität vor einer Kennzeichnung als vollständig geprüft.

## Buildzustand

Der unveränderte gemeinsame `build_repo.py` weist den Vollbuild wegen fehlender Kommentare zutreffend zurück. Die vorhandenen Kapitel wurden durch den ausdrücklich für unvollständige Lesefassungen geschriebenen `_export_draft.py` ausgegeben. Dabei wurden weder die 529 Einheiten in `units.jsonl` noch die Metadaten auf den bearbeiteten Teil verkürzt. Die strenge Gesamtvalidierung bleibt negativ; maßgeblich ist die [gesicherte Ausgabe](validation.json). Ein lokaler Commit und ein sauberer Git-Baum ersetzen diese fehlende Gesamtfertigstellung nicht.
