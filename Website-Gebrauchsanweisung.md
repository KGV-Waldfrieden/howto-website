
# Website des KGV Waldfrieden I e.V. - Gebrauchsanweisung

Stand: 16. März 2025

Dieses Dokument umfasst eine Beschreibung der Website des KGV Waldfrieden e.V. I und eine Anleitung zur Bearbeitung.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

# Überblick

Bei diesem Projekt handelt es sich um eine statische Website, d.h. alle Inhalte und Elemente der Website lieben auf einem Webserver vor und werden nicht erst beim Aufruf erzeugt.

Die Inhalte liegen primär im Format Markdown vor und in einem (öffentlich sichtbaren) Repository auf [GitHub](https://github.com/), sind aber nur als registrierter und berechtigter User bearbeitbar.

Bei GitHub ([Wikipedia-Link](https://de.wikipedia.org/wiki/GitHub)) handelt es sich um einen [Onlinedienst](https://de.wikipedia.org/wiki/Onlinedienst "Onlinedienst") zur gemeinschaftlichen [Softwareentwicklung](https://de.wikipedia.org/wiki/Softwareentwicklung "Softwareentwicklung") und [Versionsverwaltung](https://de.wikipedia.org/wiki/Versionsverwaltung "Versionsverwaltung") für Softwareprojekte. Und da eine Website auf Software basiert, bietet sich dieser Dienst zur Verwaltung an.

Technisch basiert die Website auf [GitHub Pages](https://pages.github.com/) und dem Framework [Jekyll](https://jekyllrb.com/). Jekyll ist ein sogenannter _Static (Web-)Site Generator_ ([Wikipedia-Link](https://en.wikipedia.org/wiki/Static_site_generator)) - das bedeutet, mittels dieses Werkzeugs werden aus Text-basierten 

GitHub Pages ([Wikipedia-Link](https://de.wikipedia.org/wiki/GitHub#GitHub_Pages)) bietet die Möglichkeit, statische (Website-)Inhalte im Internet zur Verfügung zu stellen ([Wikipedia-Link](https://de.wikipedia.org/wiki/Webhosting)) und ergänzt damit die Werkzeugkiste für unseren Anwendungsfall hervorragend.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

## Strukturen der Website

Auf die Website gibt es zwei strukturell unterschiedliche Sichtweisen.

### 1. Der Aufbau der Website und deren Inhalte

Die Website basiert auf einem veränderlichen Layout ("responsive design"), das sich an die Fenstergröße bzw. das verwendete Bildschirmgerät dynamisch anpasst.

 ![[/pictures/website_landing_page.png]]

Auf der Startseite (der sog. '_Landing page_') werden die jüngsten drei Posting-Auszüge angezeigt (das jeweils vollständige Posting ist durch Klick auf '_WEITERLESEN_' erreichbar) und die übrigen Posting-Sites sind über die sogenannte '_Pagination_' (zu dt. "Seitenzählung") verlinkt.

Die jeweiligen Unterseiten (Verein, Termin, Freie Gärten, FAQs, Kontakt) sind mittels der im oberen Bereich der Seite angeordneten Menü-Buttons direkt erreichbar. 

Im _Footer_-Bereich der Website finden sich außerdem noch die Links mit der Mail-Adresse und zum Impressum.

Der hierarchische Aufbau und den entsprechenden Inhalten im Überblick: 
- Logo und Name des Kleingartenvereins
- Menü
	- Verein
		- Technische Daten zum Vereinsgebiet
		- Lage des Vereins
		- Vereinssatzung
		- Der Vorstand und die Beisitzer
		- Geschäftsführung der SWG (Strom- und Wassergemeinschaft)
		- Geschichte des Vereins
		- Dokumente (Links)
	- Termine
		- Termine des laufenden Kalenderjahres
		- Links auf die archivierten Termine der vergangenen Jahre
	- Freie Gärten
		- Info ob freie Gärten verfügbar
		- Hinweis & Links auf Aufnahmeantrag für Warteliste
	- FAQs (Frequently Asked Questions = Häufige Fragen)
		- Kehrung der Schornsteine
		- Grüngut-Annahmestelle
	- Kontakt
		- Kontaktformular
		- Hinweise zum Datenschutz
- Inhalt / Content
	- Startseite
		- Begrüßung
		- Posting-Auszüge (aktuell: 3)
		- Info zu Ruhezeiten
	- sonstige Seiten
		- jeweiliger Inhalt
- Footer
	- Mail-Link
	- Impressum-Link

### 2. Die Projektseite auf GitHub

Der Verein hat einen eigenen Account auf GitHub: 
- KGV-Waldfrieden ([Link](https://github.com/KGV-Waldfrieden))

Das folgende Repository enthält die Daten der Website:
- website.github.io ([Link](https://github.com/KGV-Waldfrieden/website.github.io))

![[repository-Title.png]]

Ein weiteres Repository enthält diese Dokumentation:
- howto-website ([Link](https://github.com/KGV-Waldfrieden/howto-website))

#### Repository-Site

Im oberen Bereich der Seite befindet sich eine Menüleiste.

![[repository-Menu.png]]

Für die Bearbeitung ist primär nur die Seite mit der '_Code_'-View  relevant.

![[GitHub-Repository_1.png]]
![[GitHub-Repository_2.png]]

#### Verzeichnisbaum

Die Inhalte KGV-Website basieren auf den Inhalten der Verzeichnisse und Dateien, die in diesem Verzeichnisbaums organisiert sind. Die folgenden Abschnitte bieten eine kurze Beschreibung der hier primär relevanten Inhalte.

##### Pages
![[ordner_pages.png]]
Die Pages sind die Inhaltsseiten der Website und sind (bis auf eine Ausnahme) direkt von der Startseite (_Landing page_) über die Menü-Leiste oder den Impressum-Link im Footer erreichbar.

##### Posts / Postings
![[ordner_posts.png]]
Postings sind einzelne News oder auch Informationen, bei denen Aktualität und kurzfristige Relevanz im Vordergrund steht. Aktuell haben wir die jeweils drei aktuellsten (die jüngsten bis einschließlich heute) auf der Startseite direkt als Auszug eingebunden und verlinkt.

Es können auch bereits zukünftige Postings erstellt werden - diese werden aber erst mit Erreichen des entsprechenden Datums auf der Startseite angezeigt.

##### Bilder
![[ordner_images.png]]
In diesem Ordner sind alle Bilder, Fotos oder auch Grafiken (i.d.R. mit den Dateiendungen 'jpg', 'gif' oder 'png') abgelegt, die irgendwo auf der Website eingebunden werden. Um diese *Images* einzubinden, müssen diese selbstverständlich via **commit** Teil des _Repositories_ werden.

##### Dokumente
![[ordner_dokumente.png]]
Da auf der Website verschiedene Dokumente in verschiedenen Formaten (PDF, Word: doc/docx), aber auch als Bilddatei zur Verfügung stellen, gibt es dafür einen zentralen Ablageort. Auch für die Dokumente gilt: Um die einzubinden, d.h. auf der Website zu verlinken und auch anzuzeigen, müssen diese mittels **commit** Teil des _Repositories_ werden.

##### index.html
![[datei_index.html.png]]
Diese Datei ist per Konvention im WWW die Startseite einer Website - und so ist es auch hier. Im Gegensatz zu den ansonsten zu bearbeitenden Dateien liegt diese im HTML-Format ([Wikipedia-Link](https://de.wikipedia.org/wiki/Hypertext_Markup_Language)) vor. Wie auch das Markdown-Format ist es zwar Text-basiert, enthält aber erheblich mehr *Auszeichnungen*, die die Struktur und Gestaltung der Seite betreffen und das Lesen erschweren. Beim Blick in die Datei finden sich sämtliche Inhalte, die auf der Startseite der Website zu sehen sind, wieder.


##### Weitere Dateien und Verzeichnisse

Die übrigen Verzeichnisse und Dateien sind selbstverständlich für die Website auch relevant, weil dort Konfigurationen und beispielsweise Schriften o.ä. enthalten sind. Aber in der Regel sind dort keine Änderungen notwendig - und definitiv auch nur angeraten, wenn man weiß, was man da tut.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

# Anleitung zur Bearbeitung

Die Bearbeitung der Website folgt einem immer gleichen Schema.

| Phase     | Beschreibung                                |
| --------- | ------------------------------------------- |
| Edit.     | Bearbeiten oder Hinzufügen von Inhalten.    |
| Commit.   | Übergeben der Änderungen an das Repository. |
| Workflow. | Automatisierte Verarbeitung.                |
| Publish.  | Veröffentlichung (als GitHub-Page).         |

## Bearbeitung

Die initiale Sicht auf das Repository zeigt die '_Code_'-Ansicht mit dem bereits angesprochenen Verzeichnisbaum.

Ein Klick auf ein Verzeichnis innerhalb des Verzeichnisbaums öffnet das Verzeichnis (ähnlich wie z.B. ein Datei-Manager in Windows) und zeigt die folgende Ansicht:

![[klick_verzeichnis-ansicht.png]]

Nun geht wird es bezüglich der Bearbeitung konkreter: Ein Klick auf die Datei 'freie-gaerten.md' im gerade geöffneten Verzeichnis öffnet diese Datei.

![[klick_datei_ansicht.png]]

Die Datei wird in der '_Preview_'-Ansicht angezeigt. Diese Ansicht ähnelt stark dem, was auch auf der Website im Internet zu sehen ist. Ein weiterer Klick auf des Stift-Symbol auf der rechten Seite öffnet die '_Edit_'-Ansicht.

![[klick_datei_bearbeitung.png]]

Jetzt sind wir im '_Edit_'-Modus. Hier sehen wir jetzt die Text-Inhalte unserer ausgewählten Seite "Freie Gärten" mit den Markdown-Formatierungen.

Hier können nun Änderungen oder Ergänzungen durchgeführt werden. Die Auswirkung dieser Änderungen können gefahrlos im '_Preview_'-Modus gesichtet werden.

![[schalter_edit_und_preview.png]]

Ein Wechsel ist mit dem entsprechenden Schalter problemlos möglich.

[...]
# TODO: Beschreibung COMMIT.


### Markdown

Alle Texte auf der Website sind mittels _Markdown_ formatiert. Das bietet den großen Vorteil, dass der Text selbst lesbar bleibt und daraus über einen (in einem späteren Abschnitt beschriebenen) automatisierten Workflow die komplett formatierte Website generiert und veröffentlich werden kann.

[Markdown](https://de.wikipedia.org/wiki/Markdown) ist eine Auszeichnungssprache, mit der sich Texte auf einfache Art formatieren lassen. Einen guten Überblick über den [Einstieg in das Schreiben auf GitHub] bietet die verlinkte Site. Dort wird ein eingehenderes Verständnis ermöglicht, während der Unterabschnitt [Grundlegende Schreib- und Formatierungssyntax](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) als kompakte Referenz dienlich sein kann.


### Bilder und Dokumente

[...]
# TODO:  Einbindung beschreiben!


### Workflow

Der Workflow zur Erzeugung der Website ist automatisiert, d.h. die Änderungen brauchen nur (in GitHub) mittels '_commit_' in das Repository übergeben zu werden (vom Verständnis her ähnlich wie das 'speichern' unter Windows). Im Hintergrund wird dann automatisch der sogenannte '_Build_'-Prozess gestartet, der aus den vorhandenen Text-basierten Inhalten im Verzeichnisbaum die Website neu erzeugt.

In der Regel läuft ein solcher Prozess ohne Probleme durch und die Website wird auch gleich veröffentlicht. Das Ergebnis ist dann unter der bekannten [URL](https://www.kgv-waldfrieden-hannover.de) (Adresse der Homepage im Internet) angeschaut werden. Kommt es während des '_Build_'-Prozesses zu Fehlern, findet keine Veröffentlichung statt. Damit wird gewährleistet, das es nicht zu einer "kaputten Website" kommt. Hinweise bzgl. der Kontrolle und Fehler-Recherche werden im Anhang beschrieben Anhang.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

# Anhang

## Kontrolle des Build-Prozesses

Falls erforderlich gibt es eine Möglichkeit, Details über den _Build_-Prozess (den sog. '_Workflow_') angezeigt zu bekommen.

![[repository-Menu_Actions.png]]

Im Menü auf der Repository-Site gibt den Punkt _Actions_ und ein Klick darauf führt auf die Übersichts-Site '__Actions - All workflows__'.

![[Repository-View_Actions.png]]

Die Übersicht im rechten unteren Bereich listet die jeweils letzten _Build_-Prozess (mit Status, Startzeitpunkt, Dauer usw.) auf. In der obigen Abbildung sind die (sichtbaren) letzten beiden Build-Prozesse mit dem Status '_completed_' geendet - und so sollte es in aller Regel auch sein.

![[workflow_status_in-progress.png]]
Ein Prozess, der aktuell noch andauert, hat den Status '_in progress_' und ist mit einem gelben Kreisel-ähnlichen Symbol gekennzeichnet.

## Vorgehen im Fehlerfall

### Recherche

![[workflow_status_failure.png]]
Wird ein Prozess-Lauf mit Fehlern beendet (Status '_failure_'), wird dieser mit einem roten Kreis markiert.

In einem solchen Fall kann ein Blick in die Einzelheiten des Prozesses weiterhelfen.
Ein Klick auf '_pages build and deployment_' führt auf die _Summary_ (Zusammenfassung) des Vorgangs.

![[workflow_summary_failure.png]]

Die dort angezeigten _Annotations_ (Ausgaben) erfordern allerdings bereits ein tieferes Verständnis des _Build_-Prozesses und sind hier nur zur Information aufgezeigt.

### Bugfix oder 'Zurück auf Los'

- Änderungen können einfach gesichtet und korrigiert oder rückgängig gemacht werden.
- Wie mache ich die Änderungen einfacher sichtbar?

[...]
# TODO:  Details beschreiben!



- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
