# Sistem de monitorizare date de telemetrie IoT - stocare SQL - analiză Python - rapoarte Power BI

Acest proiect implementează un sistem complet de monitorizare și analiză a datelor IoT, având ca obiectiv detectarea anomaliilor în utilizarea CPU pe o instanță EC2. Proiectul folosește date reale din setul NAB (Numenta Anomaly Benchmark) și integrează trei componente majore: stocare SQL, analiză Python și vizualizare Power BI.

Datele utilizate provin din fișierul ec2_cpu_utilization_5f5533.csv, care conține valori reale de telemetrie AWS, cu două coloane principale: timestamp și value (utilizarea CPU). Acestea sunt procesate pentru a identifica comportamente neobișnuite, potențiale incidente sau variații semnificative în performanța sistemului.

Proiectul este structurat în trei părți:

## 1. Stocare (Backend – SQL)
Importul și organizarea datelor într-o bază de date SQL.

Pregătirea datelor pentru interogări eficiente și analize ulterioare.

## 2. Procesare și analiză (Python – Jupyter Notebook)
Curățarea și preprocesarea datelor.

Analiză exploratorie (tendințe, distribuții, variații).

Implementarea logicii de detectare a anomaliilor.

Vizualizări pentru evidențierea comportamentelor anormale.

Totul este realizat într-un notebook Jupyter pentru transparență și replicabilitate.

## 3. Vizualizare și raportare (Power BI)
Dashboard interactiv care prezintă evoluția utilizării CPU.

Evidențierea anomaliilor detectate.

Grafică intuitivă pentru interpretarea rapidă a datelor.

## © 2024 — Project created by Daria-Gabriela Iliescu.
## All rights reserved. Use, distribution, or modification of this code or associated materials is permitted only with proper attribution to the author.



Acest proiect demonstrează un flux complet de tip IoT → SQL → Python → Power BI, fiind potrivit atât pentru scopuri educaționale, cât și pentru scenarii reale de monitorizare a sistemelor.
