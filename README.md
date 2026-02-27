# HSMZ Thesis Template

Dieses Repository enthält eine LaTeX-Vorlage, die für Exposés, Hausarbeiten und Abschlussarbeiten an der Hochschule Mainz genutzt werden kann. Die Vorlage erfüllt die formalen Anforderungen, die im [Leitfaden der HS Mainz zur Anfertigung wissenschaftlicher Arbeiten (2024)](https://www.hs-mainz.de/fileadmin/Wirtschaft/Services/Pruefungsamt/pdf/Downloads/leitfaden/Leitfaden_wissenschaftlicher_Arbeiten_Deutsch.pdf) gelistet werden. 

Diese Vorlage ist im Rahmen meiner eigenen Bachelorarbeit entstanden und soll nun anderen Studierenden Zeit sparen und die Nutzung von LaTeX vereinfachen. Beispiele von fertigen Dokumenten, die meine Vorlage verwenden, bieten die folgenden Repositories:

- [ThesisHSMZ-RLTicTacToe-Expose](https://github.com/JonasBingel/ThesisHSMZ-RLTicTacToe-Expose) Repository des Exposé zu meiner Bachelorarbeit
- [ThesisHSMZ-RLTicTacToe](https://github.com/JonasBingel/ThesisHSMZ-RLTicTacToe) Repository meiner Bachelorarbeit

Hinweis: Das Logo der Hochschule Mainz kann zentral in `Metadaten.tex` ausgetauscht werden, sodass auch Studierende anderer Hochschulen die Vorlage gerne verwenden können.

## Features der Vorlage

Die folgende Auflistung enthält einige der wichtigsten Features, die meine Vorlage bietet:

- Leichter Wechsel zwischen Struktur für das Exposé und Abschlussarbeit/Hausarbeit
- Zentrale Anpassbarkeit von Metadaten (Name, Matrikelnummer, Titel, Betreuer etc.)
- [Leitfaden zur Anfertigung von Abschlusarbeiten der Hochschule Mainz (2020)](https://www.hs-mainz.de/studium/services/wirtschaft/pruefungsmanagement/downloads/) wird eingehalten
    - Titelseite mit allen geforderten Angaben
    - Schriftbild und Ränder
    - Formale Ordnung und Reihenfolge
    - Seitennummerierung
    - Vorlage für eidesstattliche Erklärung und Sperrvermerk der Hochschule Mainz
    - Anhang mit Anhangsverzeichnis und fortlaufender römischer Nummerierung
- Verzeichnisse für
    - Abbildungen
    - Tabellen
    - Abkürzungen
    - Symbole
    - Formeln
    - Algorithmen
    - Listing (Quellcode)
- Literaturverzeichnis mit BibLaTeX und Voreinstellungen für IEEE und APA
- Listing zur Darstellung von Quellcode (über mehrere Seiten) mittels `minted`
- Darstellung von Algorithmen mittels `algorithm2e`
- Referenzieren von Gleitumgebungen mittels `Varioref` und `Cleverref`
- Verwalten von Kommentaren und offenen Punkten mittels `todonotes`
- Pakete zum Erstellen guter wissenschaftlicher Tabellen (über mehrere Seiten)
- Automatisch generierte PDF-Bookmarks für die einzelnen Abschnitte

## Anleitung zur Verwendung

Voraussetzung für die Nutzung dieser Vorlage ist ein grundlegendes Verständnis von LaTeX.
Einen guten Einstieg in LaTeX bietet beispielsweise dieses [Tutorial von Overleaf](https://www.overleaf.com/learn/latex/Tutorials).

1. Repository als Zip herunterladen und in favorisierten LaTeX-Editor einbinden
2. In der Datei 00_Allgemein/Metadaten.tex die Metadaten aktualisieren (Name, Matrikelnummer, Titel etc.)
3. Entsprechend der Verwendung eine Hauptdatei wählen 
    1. Bei einem Expose ist `Expose.tex` zu verwenden und `Arbeit.tex` zu löschen
    2. Bei einer Haus-/Bachelor-/Masterarbeit ist `Arbeit.tex` zu verwenden und `Expose.tex` zu löschen
4. Die gewählte Hauptdatei durchlesen und ggf. benötigte Abschnitte einblenden (z.B. Sperrvermerk)
5. Zugehörige Datei im Verzeichnis 02_Textteil ansehen und losschreiben 🙂

## Struktur der Vorlage

Dieser Abschnitt bietet einen Überblick über die Struktur der Vorlage und erklärt den Zweck der einzelnen Dateien. In den Dateien selbst ist jeweils ein Kommentar enthalten, der konkretere Informationen und Hinweise bietet.

`Expose.tex` Haupdatei für ein Expose, die dem LaTeX-Kompiler übergeben wird

`Arbeit.tex` Haupdatei für eine Arbeit, die dem LaTeX-Kompiler übergeben wird

Verzeichnis `00_Allgemein` enthält alle Dateien, die zur Konfiguration von TeX und der Vorlage verwendet werden

- `Befehle.tex` Definition von Custom-Anweisungen
- `Metadaten.tex` Metadaten zur Arbeit, Autor, Betreuer und Hochschule (inkl. Logo)
- `Nomenklatur.tex` Nomenklatur, d.h. verwendete Symbole in der Arbeit (Symbolverzeichnis)
- `Packages.tex` LaTeX-Packages und deren Konfiguration
- `ToDo.tex` Eine To-do-Liste sowie allgemeine To-dos, die mittels Package `todonotes` erstellt werden

Verzeichnis `01_Vortext` enthält alle Dateien/Seiten, die dem eigentlichen Textteil vorangestellt sind

- `01_Sperrvermerk.tex` Optionaler Sperrvermerk, der die erste Seite bildet
- `02_Titelseite.tex` Titelseite des Exposes bzw. der Arbeit
- `03_Erklaerung.tex` Eidesstattliche Erklärung
- `04_ManagementSummary.tex` Management Summary (Abstract) zur Arbeit
- `05_Verzeichnisse.tex` Konfiguration der Verzeichnisse, die angezeigt werden sollen und deren Reihenfolge
- `06_Abkuerzungen.tex` Abkürzungen, die in der Arbeit genutzt und im Abkürzungsverzeichnis gelistet werden

Verzeichnis `02_Texttteil` enthält den eigentlichen Inhalt der Arbeit

- `00_Inhalt_Expose.tex` Vorlage für ein Expose
- `00_Inhalt_Arbeit.tex` Haupdatei der zu erstellenden Arbeit (enthält Beispiele zur Nutzung der Features der Vorlage)

Verzeichnis `03_Nachtext` enthält alle Dateien, die den Anhang der Arbeit bilden 

- `01_Anhang.tex` definiert den Anhang und bindet ggf. weitere Seiten ein

Verzeichnis `04_Artefakte` enthält alle Artefakte, die in der Arbeit verwendet werden. Zur besseren Übersichtlichkeit gibt es Unterverzeichnisse für die einzelnen Artefaktarten.

## Nutzungshinweise

Die Nutzung der Vorlage ist und bleibt vollkommen kostenfrei.

Im PDF-Export eurer Arbeit muss selbstverständlich nicht auf diese Vorlage verwiesen werden. Meine Bitte ist jedoch in eurem LaTeX-Quellcode auf diese Vorlage zu verweisen, sodass andere sie ebenfalls nutzen können.

## Verbesserungen

Verbesserungsvorschläge können gerne als Issue oder Pull-Request eingereicht werden.

## Empfehlungen zur Verwendung

Beim Schreiben meiner eigenen Bachelorarbeit mit dieser LaTeX-Vorlage waren insbesondere zwei Anwendungen sehr hilfreich, die ich daher hier kurz empfehlen möchte:

- Overleaf - Online LaTeX-Editor, der es euch erspart LaTeX lokal zu installieren und Pakete zu verwalten
- Zotero mit dem Add-On “Better BibTeX for Zotero” - Verwaltung der Literatur und Export als BibLaTeX-Datei, um das Literaturverzeichnis einfach zu erstellen

## Kurzanleitung Nutzung in Overleaf

Wenn ihr Overleaf als LaTeX-Editor verwenden möchtet, könnt ihr folgende Anleitung verwenden, um direkt loszuschreiben: 

1. Dieses Repository als Zip-Datei herunterladen
2. Overleaf-Account anlegen
3. In Overleaf mittels `New Project` ein neues Projekt anlegen und und anschließend bei `Upload Project` die heruntergeladene Zip-Datei auswählen

![Overleaf New Project](https://imgur.com/W0XkLiT.png)
    
4. In den Einstellungen des Projekts bei der Option `Main document` entweder `Arbeit.tex` oder `Expose.tex` wählen und die andere Datei löschen


![Overleaf - Choose File](https://imgur.com/ybWe0rj.png)   
5. Projekt rekompilieren und losschreiben 🙂


## Nutzungbedingungen des Logos der Hochschule Mainz

Dieser Abschnitt ist eine Kopie der [offiziellen Nutzungsbedingungen für das Logo der Hochschule Mainz](https://www.hs-mainz.de/pressemedien/logo/). Er dient hier nur zu Referenzzwecken. Innerhalb dieser Vorlage ist das Logo für die Verwendung durch Studierende und Doktoranden vorgesehen.

### Wort-Bild-Marke der Dachmarke

Das Logo der Hochschule Mainz besteht aus der Wort-Marke „Hochschule Mainz“, der abstrakten Bild-Marke „M“, sowie dem internationalen Zusatz „University of Applied Sciences“. Die Wort-Marke steht in der Regel auf Medien links oben. Die Hochschule Mainz verwendet übergreifend ein Logo (Wort-Bild-Marke). Die Möglichkeit der Fachbereichskennungen entnehmen Sie bitte dem Corporate Design-Manual.

### Wer darf das Logo wann und wie nutzen?

Beim Logo der Hochschule Mainz handelt es sich um eine Wort-Bild-Marke. Sie genießt Markenschutz. Die Nutzungs- und Verwertungsrechte liegen ausschließlich bei der Hochschule Mainz.

Es dürfen lediglich die von der Hochschule Mainz erstellten Vorlagen genutzt werden. Das Logo muss stets scharf und sauber dargestellt sein und darf nicht verzerrt werden. Eine andere Anordnung, das Nachzeichnen oder Nachsetzen der Wort-Bild-Marke sind nicht zulässig. Die Regeln des Corporate Designs der Hochschule Mainz sind zu berücksichtigen.

### Dienstliche Verwendung

Das Logo der Hochschule Mainz darf von allen Beschäftigten, Professorinnen und Professoren, Lehrbeauftragten sowie gastweise tätigen Lehrkräften genutzt werden. Es wird im dienstlichen Schriftverkehr eingesetzt, z.B. auf Briefen, Visitenkarten, Berichten, Protokollen und Formularen.

Das Logo findet außerdem Anwendung in Printmedien, im Internet auf den offiziellen Webseiten sowie auf Merchandising-Produkten.

Die Nutzung des Logos ist erwünscht bei Postern, Flyern und Power Point-Präsentationen sowie sonstigen Präsentationen, die im Rahmen von Lehre und Forschung sowie der dienstlichen Tätigkeit erstellt werden. Dies gilt z.B. für Veranstaltungen, auf denen Mitarbeiterinnen und Mitarbeiter als Repräsentanten der Hochschule Mainz auftreten und/oder Forschungsergebnisse präsentieren. Die Nutzung des Logos ist außerdem erwünscht in Publikationen, die im dienstlichen Rahmen und Auftrag erstellt und/oder herausgegeben werden.

### Verwendung durch Studierende und Promovierende

Die Logo-Nutzung ist auch Studierenden oder Promovierenden im Rahmen des Studiums gestattet. Hierzu zählt insbesondere die Nutzung des Logos auf Postern, Flyern und Power Point- Präsentationen sowie Haus- und Abschlussarbeiten. Ausgenommen ist die Nutzung des Logos im Rahmen der Veröffentlichung von Haus- und Abschlussarbeiten, wenn die entsprechende Prüfungsleistung nicht bestanden wurde.

Die Logo-Nutzung ist auch studentischen Projekten an der Hochschule Mainz gestattet, wenn

das Projekt als Studienleistung anerkannt wird.
das Projekt durch Haushaltsmittel der Hochschule Mainz unterstützt wird.
es eine vertragliche Vereinbarung zwischen dem Projektteam und der Hochschule Mainz gibt.

### Verwendung durch Kooperationspartner

Die Nutzung des Logos der Hochschule Mainz durch Kooperationspartner ist zulässig, wenn es sich um eine vertraglich festgelegte Kooperation handelt und der Kooperationsvertrag eine solche Nutzung ausdrücklich vorsieht. Im Rahmen der Vertragsgestaltung sind die näheren Bestimmungen der Nutzung festzulegen, insbesondere

dass sich die Hochschule Mainz das Recht vorbehält, die Nutzungserlaubnis jederzeit zu widerrufen, wenn die Nutzung nicht der vertraglich festgelegten Logo-Nutzung entspricht.
dass nur die Vorlagen der Hochschule Mainz genutzt und das Logo nicht verändert oder verfälscht werden dürfen bzw. darf.
dass grundsätzlich das im CD- Manual der Hochschule Mainz zum Download zur Verfügung gestellte Logo zu nutzen ist.

### Verwendung durch Dritte

Sollte keine der vorgenannten Voraussetzungen zur Logo-Nutzung erfüllt sein, so bedarf die Verwendung des Logos einer schriftlichen Zustimmung. Sie wird von der Abteilung Presse und Kommunikation der Hochschule Mainz auf Anfrage per E-Mail erteilt. Dieser muss das entsprechende Kommunikationsmittel vor der Nutzung des Logos zur Überprüfung der Einhaltung der Corporate Design-Vorgaben vorgelegt werden.

### Zustimmung

Eine Zustimmung setzt voraus, dass die Logo-Nutzung im Zusammenhang mit den Aufgaben und/oder Interessen der Hochschule Mainz steht und keine Beeinträchtigung des Ansehens der Hochschule durch die Nutzung zu erwarten ist. Die Hochschule Mainz kann eine einmal erteilte Zustimmung jederzeit ohne Angabe von Gründen zurückziehen.