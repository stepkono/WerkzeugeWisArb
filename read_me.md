LaTeX-Unterlagen
=================

In diesem Repository befinden sich die LaTeX-Unterlagen zum Modul.

Inhalt
------

Der Inhalt entspricht dem Text der Aufgabe 2 des Moduls. Es kann sinnvoll sein, sich die PDF zur Aufgabe 2 noch einmal anzusehen.

PDF erstellen
-------------

Das Erstellen der PDF ist schnell und einfach:

- Zuerst LaTeX installieren: <https://tug.org/texlive/>
- PDF mit `pdflatex` erstellen (ggf. mehrfach ausführen):

```text
pdflatex ./task.tex
```

- Alternativ mit `latexmk` (empfohlen):

```text
latexmk -pdf ./task.tex
```

Wichtig
-------

**Achtung:** LaTeX erzeugt Hilfsdateien wie `.aux`, `.log`, `.fdb_latexmk` und `.fls`. Vor dem Commit sollten diese Dateien entfernt werden. Beispiel:

```text
rm -f *.aux *.log *.fdb_latexmk *.fls
```
