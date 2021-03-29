**FHIR-Beispiele zum E-Rezept - Version**  **1.0.1 vom**** 05.03.2021**

In diesem Projekt stellt der DAV Beispiele für die bei der Verarbeitung von E-Rezepten auftretenden Dateien in der Apotheke und dem Apothekenrechenzentrum zur Verfügung. Es wurde darauf geachtet, dass die zu einem Beispiel gehörenden Dateien fachlich und technisch zusammenpassen und soweit wie möglich realistische Informationen enthalten.

Noch zu ergänzen: Nutzung der Referenzimplementierung

Der folgende Workflow wird betrachtet:

![workflow.png](workflow.png)

Zu jedem Beispiel werden folgende Dateien zur Verfügung gestellt:

**A) Verordnung und signierte Verordnung**

Als Verordnungen wurden von der KBV im Projekt [https://simplifier.net/eRezept](https://simplifier.net/eRezept) veröffentlichte Beispiele genutzt. Für die Verwendung in den vorliegenden Beispiel-Verordnungs\_Bundles mussten die Verordnungen in einzelnen Feldern passend zum Task auf dem E-Rezept-Fachdienst geändert werden (insbesondere Rezept-ID, Ausstellungsdatum). Die Signatur erfolgte mit …

**B) Medication Dispense**

Die Medication Dispense wird in der Apotheke aus Daten der Verordnung bzw. der Abgabedaten erzeugt und um Telematik-ID (aus der SMC-B) und Verfalldatum (aus den securpharm-Daten) ergänzt. Beim Abruf der Quittung muss die Medication Dispense an den E-Rezept-Fachdienst übergeben werden.

In den Beispielen wurde die Medication Dispense vom DAV erstellt.

**C) Quittung des E-Rezept-Fachdienstes**

Die Quittung wurde durch den E-Rezept-Fachdienst inkl. eingebetteter Signatur erstellt.

**D) Abgabedaten und signierte Abgabedaten**

Die Abgabedaten wurden vom DAV erstellt und mit … signiert.

**E) Abrechnungsdaten und TA7-Daten**

Die Abrechnungsdaten und TA7-Daten wurden fachlich von Noventi bereitgestellt und technisch von der gevko in FHIR-Dateien umgesetzt.

**Ergänzende Informationen zu den Abgabedaten bei den einzelnen Beispielen**

**1) PZN-Verordnung Nr. 1**

Merkmal: Erfüllung Rabattvertrag

Signatur: Zertifikat … (entsprechend der Signatur mit einer SMC-B)

Weitere Beispiele folgen.


