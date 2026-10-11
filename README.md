# Psychologie als Wissenschaft

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/jvanvinkenroye/psychologie-als-wissenschaft/main/psychologie_als_wissenschaft.md)

Interaktiver LiaScript-Kurs: Einführung in die Psychologie als Wissenschaft und in
die Grundlagen empirischer Forschung (Intuition und ihre Grenzen, wissenschaftliche
Methode, Erklärungsebenen, Vierfeldertafel, Variablentypen, Hypothesen,
Falsifikation, Güte von Hypothesen) mit Übungen und Abschlussquiz.

## Kurs öffnen

Direkt im Browser, ohne Installation:

<https://liascript.github.io/course/?https://raw.githubusercontent.com/jvanvinkenroye/psychologie-als-wissenschaft/main/psychologie_als_wissenschaft.md>

Antworten und Fortschritt werden nur lokal im Browser gespeichert.

## SCORM-Paket für Moodle

Bei jedem Push auf `main` erzeugt eine GitHub Action ein SCORM-1.2-Paket
(Preset Moodle 4/5). Es liegt unter *Actions* als Artefakt bereit. Bei einem
Tag `v*` (z. B. `v1.1.0`) wird es zusätzlich an ein Release angehängt.

Lokal exportieren:

```bash
PUPPETEER_SKIP_DOWNLOAD=1 npx @liascript/exporter \
  -i psychologie_als_wissenschaft.md -f presets --moodle4 \
  --scorm-organization "Psychologie als Wissenschaft" \
  --scorm-typicalDuration PT1H30M0S \
  -o export/psychologie_als_wissenschaft_moodle
```

## Bearbeiten

Der Kurs ist eine einzige Markdown-Datei: `psychologie_als_wissenschaft.md`.
Vorschau lokal mit `npx @liascript/devserver --input psychologie_als_wissenschaft.md --live`
oder der VS-Code-Erweiterung „LiaScript-Preview“.

Hinweis zu `version:` im Kurskopf: Eine Änderung der Hauptversion (z. B. 1.x -> 2.0.0)
setzt den gespeicherten Fortschritt der Lernenden zurück; nur bei strukturellen
Änderungen an Quizzen erhöhen.

## Autor

Jan Vanvinkenroye
