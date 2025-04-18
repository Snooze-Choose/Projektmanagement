#

**Über arc42**

arc42, das Template zur Dokumentation von Software- und
Systemarchitekturen.

Template Version 8.2 DE. (basiert auf AsciiDoc Version), Januar 2023

Created, maintained and © by Dr. Peter Hruschka, Dr. Gernot Starke and
contributors. Siehe <https://arc42.org>.

# Einführung und Ziele {#section-introduction-and-goals}

## Aufgabenstellung {#\_aufgabenstellung}

Ein bestehender, veralteter Webshop soll grundlegend überarbeitet werden, um den steigenden Anforderungen des Marktes gerecht zu werden. Ziel ist es, eine moderne, benutzerfreundliche und leistungsfähige E-Commerce-Plattform bereitzustellen, die ein optimales Einkaufserlebnis für Kundinnen und Kunden bietet und gleichzeitig die internen Betriebsabläufe effizient unterstützt.
Die vollständige Konzeption und Umsetzung des neuen Systems erfolgt durch ein internes Softwareentwicklungsteam. Externe Partner oder Dienstleister sind in diesen Prozess nicht eingebunden.
Das neue System soll alle zentralen E-Commerce-Funktionen abdecken. Dazu gehören unter anderem die Nutzerregistrierung und -verwaltung, eine leistungsstarke Produktsuche, Warenkorbfunktionen, ein durchgängiger Checkout-Prozess, Bestellbestätigungen sowie ein administrativer Bereich zur Artikelpflege und zur Verwaltung von Bestellungen.
Technisch wird das System plattformunabhängig und hoch skalierbar konzipiert, um auch bei stark schwankender Last zuverlässig zu funktionieren. Der Betrieb erfolgt in einer Azure-basierten Cloud-Infrastruktur, um eine hohe Verfügbarkeit sowie einfache Wartung und Erweiterbarkeit zu gewährleisten

## Projektziele {#\_qualit_tsziele}

Die Projektziele finden sich im Backlog
[text](https://github.com/orgs/Snooze-Choose/projects/6/views/3)

## Qualitätsziele {#\_qualit_tsziele}

## Stakeholder {#\_stakeholder}

## Stakeholder-Tabelle

| Name             | Rolle           | Interesse am Projekt                             | Einfluss auf das Projekt | Erwartungshaltung                                            |
| ---------------- | --------------- | ------------------------------------------------ | ------------------------ | ------------------------------------------------------------ |
| Christoph Loeser | Auftraggeber    | Erfolgreiche Umsetzung im Budget und Zeitrahmen  | Hoch                     | Transparente Kommunikation, Einhaltung von Budget & Terminen |
| Max Mustermann   | Kunden          | Benutzerfreundliches und funktionales Endprodukt | Mittel                   | Hohe Qualität, intuitive Bedienung, schneller Support        |
| IT-Team          | Administratoren | Stabile, wartbare und sichere Systemumgebung     | Gering                   | Technische Dokumentation, einfache Wartbarkeit, Sicherheit   |

# Randbedingungen {#section-architecture-constraints}

# Kontextabgrenzung {#section-context-and-scope}

## Fachlicher Kontext {#\_fachlicher_kontext}

**\<Diagramm und/oder Tabelle>**

**\<optional: Erläuterung der externen fachlichen Schnittstellen>**

## Technischer Kontext {#\_technischer_kontext}

**\<Diagramm oder Tabelle>**

**\<optional: Erläuterung der externen technischen Schnittstellen>**

**\<Mapping fachliche auf technische Schnittstellen>**

# Lösungsstrategie {#section-solution-strategy}

# Bausteinsicht {#section-building-block-view}

## Whitebox Gesamtsystem {#\_whitebox_gesamtsystem}

**_\<Übersichtsdiagramm>_**

Begründung

: _\<Erläuternder Text>_

Enthaltene Bausteine

: _\<Beschreibung der enthaltenen Bausteine (Blackboxen)>_

Wichtige Schnittstellen

: _\<Beschreibung wichtiger Schnittstellen>_

### \<Name Blackbox 1> {#\_\_name_blackbox_1}

_\<Zweck/Verantwortung>_

_\<Schnittstelle(n)>_

_\<(Optional) Qualitäts-/Leistungsmerkmale>_

_\<(Optional) Ablageort/Datei(en)>_

_\<(Optional) Erfüllte Anforderungen>_

_\<(optional) Offene Punkte/Probleme/Risiken>_

### \<Name Blackbox 2> {#\_\_name_blackbox_2}

_\<Blackbox-Template>_

### \<Name Blackbox n> {#\_\_name_blackbox_n}

_\<Blackbox-Template>_

### \<Name Schnittstelle 1> {#\_\_name_schnittstelle_1}

...

### \<Name Schnittstelle m> {#\_\_name_schnittstelle_m}

## Ebene 2 {#\_ebene_2}

### Whitebox _\<Baustein 1>_ {#\_whitebox_emphasis_baustein_1_emphasis}

_\<Whitebox-Template>_

### Whitebox _\<Baustein 2>_ {#\_whitebox_emphasis_baustein_2_emphasis}

_\<Whitebox-Template>_

...

### Whitebox _\<Baustein m>_ {#\_whitebox_emphasis_baustein_m_emphasis}

_\<Whitebox-Template>_

## Ebene 3 {#\_ebene_3}

### Whitebox \<\_Baustein x.1\_\> {#\_whitebox_baustein_x_1}

_\<Whitebox-Template>_

### Whitebox \<\_Baustein x.2\_\> {#\_whitebox_baustein_x_2}

_\<Whitebox-Template>_

### Whitebox \<\_Baustein y.1\_\> {#\_whitebox_baustein_y_1}

_\<Whitebox-Template>_

# Laufzeitsicht {#section-runtime-view}

## _\<Bezeichnung Laufzeitszenario 1>_ {#\_\_emphasis_bezeichnung_laufzeitszenario_1_emphasis}

- \<hier Laufzeitdiagramm oder Ablaufbeschreibung einfügen>

- \<hier Besonderheiten bei dem Zusammenspiel der Bausteine in diesem
  Szenario erläutern>

## _\<Bezeichnung Laufzeitszenario 2>_ {#\_\_emphasis_bezeichnung_laufzeitszenario_2_emphasis}

...

## _\<Bezeichnung Laufzeitszenario n>_ {#\_\_emphasis_bezeichnung_laufzeitszenario_n_emphasis}

...

# Verteilungssicht {#section-deployment-view}

## Infrastruktur Ebene 1 {#\_infrastruktur_ebene_1}

**_\<Übersichtsdiagramm>_**

Begründung

: _\<Erläuternder Text>_

Qualitäts- und/oder Leistungsmerkmale

: _\<Erläuternder Text>_

Zuordnung von Bausteinen zu Infrastruktur

: _\<Beschreibung der Zuordnung>_

## Infrastruktur Ebene 2 {#\_infrastruktur_ebene_2}

### _\<Infrastrukturelement 1>_ {#\_\_emphasis_infrastrukturelement_1_emphasis}

_\<Diagramm + Erläuterungen>_

### _\<Infrastrukturelement 2>_ {#\_\_emphasis_infrastrukturelement_2_emphasis}

_\<Diagramm + Erläuterungen>_

...

### _\<Infrastrukturelement n>_ {#\_\_emphasis_infrastrukturelement_n_emphasis}

_\<Diagramm + Erläuterungen>_

# Querschnittliche Konzepte {#section-concepts}

## _\<Konzept 1>_ {#\_\_emphasis_konzept_1_emphasis}

_\<Erklärung>_

## _\<Konzept 2>_ {#\_\_emphasis_konzept_2_emphasis}

_\<Erklärung>_

...

## _\<Konzept n>_ {#\_\_emphasis_konzept_n_emphasis}

_\<Erklärung>_

# Architekturentscheidungen {#section-design-decisions}

# Qualitätsanforderungen {#section-quality-scenarios}

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Qualitätsanforderungen](https://docs.arc42.org/section-10/) in
der online-Dokumentation (auf Englisch!).

## Qualitätsbaum {#\_qualit_tsbaum}

## Qualitätsszenarien {#\_qualit_tsszenarien}

# Risiken und technische Schulden {#section-technical-risks}

# Glossar {#section-glossary}

+-----------------------+-----------------------------------------------+
| Begriff | Definition |
+=======================+===============================================+
| _\<Begriff-1>_ | _\<Definition-1>_ |
+-----------------------+-----------------------------------------------+
| _\<Begriff-2_ | _\<Definition-2>_ |
+-----------------------+-----------------------------------------------+
