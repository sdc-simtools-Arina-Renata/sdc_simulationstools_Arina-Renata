# Projektidee – Therapieplätze & Wartezeiten (Monte-Carlo-Modell)
# Stand: 2024 – Region Nordbayern
________________________________________________________________
# Thema

Analyse der Versorgungssituation im Bereich psychologischer Psychotherapie in Nordbayern und Simulation der Wartezeiten auf Therapieplätze im Jahr 2024.

________________________________________________________________

# Problemstellung

Die Versorgung mit ambulanten psychotherapeutischen Leistungen ist regional stark begrenzt. 
In vielen Städten und Landkreisen treten:
	•	lange Wartezeiten (mehrere Wochen bis Monate),
	•	Versorgungsengpässe,
	•	Ungleichgewicht zwischen Nachfrage und verfügbaren Therapieplätzen,
	•	und fehlende oder unzureichende Maßnahmen zur Verkürzung der Wartezeit
auf.

Diese Situation stellt sowohl für Betroffene als auch für die Gesundheitsversorgung eine hohe Belastung dar.

________________________________________________________________

# Modellansatz (Monte-Carlo-Simulation)

Zur Analyse wird ein Warteschlangensystem modelliert:

Systemkomponenten
	•	Ankünfte: neue Patient*innen, die einen Therapieplatz suchen
	•	Behandlungsdauer: Länge der Therapie (z. B. 10–60 Sitzungen; wird als Zufallsvariable modelliert)
	•	Kapazität: verfügbare Sitzungen pro Woche
	•	Anzahl Therapeut*innen × Stunden pro Woche
	•	Auslastung: niedrig, mittel, hoch
	•	Wartezeit = Zeitspanne zwischen Erstkontakt und Therapiebeginn

Zielgrößen
	•	Wie wahrscheinlich ist eine Wartezeit
	•	über 3 Monate?
	•	über 6 Monate?
	•	Wie entwickelt sich der Rückstau („Warteliste“) im Jahresverlauf?

Simulationslauf
	•	Ein Simulationslauf entspricht einem Zeitraum von 1 Jahr (365 Tage)
	•	Durch Wiederholung vieler Läufe entsteht eine Monte-Carlo-Verteilung der Wartezeiten

________________________________________________________________

# Annahmen / Recherchebasis

Für das Modell werden recherchiert, geschätzt oder aus Quellen abgeleitet:
	•	Anzahl der Psychotherapeut*innen pro Region
	•	Kapazität pro Therapeut*in (z. B. 20–30 Therapie-Stunden/Woche)
	•	durchschnittliche Therapiedauer (z. B. 20–60 Sitzungen)
	•	Anzahl der wöchentlichen Neuanmeldungen
	•	Auslastung (in vielen Regionen > 90 %)
	•	Therapieabbruchsrate (optional)

Diese Werte werden als Parameter im Modell festgelegt.

________________________________________________________________

# Faktoren / Merkmale

Für die Interpretation können zusätzliche Faktoren berücksichtigt werden:
	•	Krankenkassenstatus
(gesetzlich vs. privat → oft große Unterschiede in Wartezeit und Platzverfügbarkeit)
	•	Betroffene Gruppen
z. B. Erwachsene, Jugendliche, Notfälle

Diese Faktoren fließen optional in Szenarien oder Diskussion ein.

________________________________________________________________

# Bedingungen / Szenarien

Für die Simulation können unterschiedliche Szenarien aufgebaut werden:

Szenario A – Status quo
	•	aktuelle Kapazität und Nachfrage
	•	Präsenztherapie, 1:1-Behandlung

Szenario B – Kapazitätserhöhung
	•	mehr Therapeut*innen oder mehr Stunden/Woche

Szenario C – Kürzere Therapiedauer
	•	durchschnittliche Sitzungszahl sinkt (z. B. -10 %)

Szenario D – Kombination
	•	mehr Kapazität + effizientere Abläufe

Szenario E – Digitale Therapie / Hybrid
	•	zusätzliche Online-Sitzungen als Kapazitätserweiterung

Diese Szenarien werden per Monte-Carlo simuliert und verglichen.

________________________________________________________________

# Kurzfazit der Projektidee

Die Projektarbeit untersucht, wie gut die psychotherapeutische Versorgung in Nordbayern die Nachfrage abdeckt und wie lange Patient*innen realistisch auf einen Therapieplatz warten.
Mit einem Monte-Carlo-Warteschlangenmodell werden Wartezeiten simuliert, Engpässe sichtbar gemacht und mögliche Maßnahmen bewertet, die zu einer Verkürzung der Wartezeiten führen können.





- bullet
# hi / Überschrift
bvxh