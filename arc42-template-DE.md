#

**Über arc42**

arc42, das Template zur Dokumentation von Software- und
Systemarchitekturen.

Template Version 8.2 DE. (basiert auf AsciiDoc Version), Januar 2023

Created, maintained and © by Dr. Peter Hruschka, Dr. Gernot Starke and
contributors. Siehe <https://arc42.org>.

# Einführung und Ziele {#section-introduction-and-goals}

## Aufgabenstellung {#\_aufgabenstellung}

Ziel ist es, eine moderne, benutzerfreundliche und leistungsfähige E-Commerce-Plattform bereitzustellen, die ein optimales Einkaufserlebnis für Kundinnen und Kunden bietet und gleichzeitig die internen Betriebsabläufe effizient unterstützt.
Die vollständige Konzeption und Umsetzung des neuen Systems erfolgt durch ein internes Softwareentwicklungsteam. Externe Partner oder Dienstleister sind in diesen Prozess nicht eingebunden.
Das neue System soll alle zentralen E-Commerce-Funktionen abdecken. Dazu gehören unter anderem die Nutzerregistrierung und -verwaltung, eine leistungsstarke Produktsuche, Warenkorbfunktionen, ein durchgängiger Checkout-Prozess, Bestellbestätigungen sowie ein administrativer Bereich zur Artikelpflege und zur Verwaltung von Bestellungen.
Technisch wird das System plattformunabhängig und hoch skalierbar konzipiert, um auch bei stark schwankender Last zuverlässig zu funktionieren. Der Betrieb erfolgt in einer Azure-basierten Cloud-Infrastruktur, um eine hohe Verfügbarkeit sowie einfache Wartung und Erweiterbarkeit zu gewährleisten.

## Projektziele {#\_qualit_tsziele}

Die Projektziele finden sich im [hier](https://github.com/Snooze-Choose/Projektmanagement/issues?q=is%3Aissue%20state%3Aopen%20label%3Aepic).

## Stakeholder {#\_stakeholder}

## Stakeholder-Tabelle

| Name             | Rolle           | Interesse am Projekt                             | Einfluss auf das Projekt | Erwartungshaltung                                            |
| ---------------- | --------------- | ------------------------------------------------ | ------------------------ | ------------------------------------------------------------ |
| Christoph Loeser | Auftraggeber    | Erfolgreiche Umsetzung im Budget und Zeitrahmen  | Hoch                     | Transparente Kommunikation, Einhaltung von Budget & Terminen |
| Max Mustermann   | Kunden          | Benutzerfreundliches und funktionales Endprodukt | Mittel                   | Hohe Qualität, intuitive Bedienung, schneller Support        |
| IT-Team          | Administratoren | Stabile, wartbare und sichere Systemumgebung     | Gering                   | Technische Dokumentation, einfache Wartbarkeit, Sicherheit   |

# Randbedingungen {#section-architecture-constraints}

## Technische Randbedingungen {#\_technische_Randbedingungen}

| Komponente        | Technologie           |
| ----------------- | --------------------- |
| Backend           | C# .NET Web API Core  |
| ORM               | Entity Framework Core |
| Datenbank         | PostgreSQL            |
| Frontend          | TypeScript + Vue.js   |
| Service Discovery | .NET Aspire           |
| Containerisierung | Docker                |

## Organisatorische Randbedingungen {#\_organisatorische_Randbedingungen}

Die Entwicklung des Systems erfolgt nach dem Scrum-Vorgehensmodell.
Sprints haben eine feste Dauer von zwei Wochen.
Rollen wie Product Owner, Scrum Master und Entwicklungsteam sind definiert und besetzt.
Die Sprintplanung, Reviews und Retrospektiven finden regelmäßig gemäß dem Scrum-Framework statt.

# Kontextabgrenzung {#section-context-and-scope}
Zur präzisen Definition der fachlichen Kontextabrenzung wurde ein UML-Diagramm erstellt, welches sämtliche Kommunikationsbeziehungen mit dem System festlegt.

[![Fachlicher Kontext](images/fachlicher_context.png)](images/fachlicher_context.png)

# Lösungsstrategie {#section-solution-strategy}

# Bausteinsicht {#section-building-block-view}

## Whitebox Gesamtsystem {#\_whitebox_gesamtsystem}

[![Whitebox Gesamtsystem](images/whitebox.png)](images/whitebox.png)

[![Blackbox Gesamtsystem](images/blackbox.png)](images/blackbox.png)

# Laufzeitsicht {#section-runtime-view}

## _\<Zustände der Bestellung>_ {#\_\_emphasis_zustand_der_bestellung_emphasis}

[![Zustand der Bestellung](images/zustand_bestellung.png)](images/zustand_bestellung.png)

## _\<Bezeichnung Laufzeitszenario 2>_ {#\_\_emphasis_bezeichnung_laufzeitszenario_2_emphasis}

...

## _\<Bezeichnung Laufzeitszenario n>_ {#\_\_emphasis_bezeichnung_laufzeitszenario_n_emphasis}

...

# Verteilungssicht {#section-deployment-view}

[![Grobarchitektur](images/architektur.png)](images/architektur.png)

# Querschnittliche Konzepte {#section-concepts}

## _\<Konzept 1>_ {#\_\_emphasis_konzept_1_emphasis}

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

### Risiko: Geringe Nutzerakzeptanz des Shops

- **Beschreibung:** Es besteht das Risiko, dass der entwickelte Shop von der Zielgruppe nicht wie erwartet angenommen wird. Mögliche Ursachen können eine unzureichende Nutzerführung, fehlende Funktionen, mangelnde Performance oder ein nicht zielgruppengerechtes Design sein.
- **Auswirkungen:** Geringe Nutzerzahlen, niedrige Conversion-Rate, wirtschaftlicher Misserfolg des Produkts. Hoher Anpassungsaufwand nach dem Go-live zur Nachbesserung.
- **Gegenmaßnahmen:**
  - Frühzeitige Einbindung von Endnutzern durch Usability-Tests und Feedbackzyklen (z. B. Prototypentests, A/B-Tests).
  - Iterative Entwicklung mit MVP-Ansatz und klar definierten Akzeptanzkriterien.
  - Analyse von Konkurrenzprodukten und Nutzerverhalten.
- **Technische Schulden:** Möglicherweise müssen grundlegende Architektur- oder Designentscheidungen überarbeitet werden, falls sich im Live-Betrieb fundamentale Nutzungsprobleme zeigen. Dies kann zu erhöhtem Refactoring-Aufwand führen.

# Glossar {#section-glossary}
