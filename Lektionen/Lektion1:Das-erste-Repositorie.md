# Erste Schritte

## Das erste Repository

```{.bash}
mkdir GitWorkshop
cd GitWorkshop

 # Initialisieren des Repositorys
git init

 # Status Ausgeben
git status
```

## Erster Commit

Kopiere den Inhalt der Git-Workshop.zip in den soeben initiierten GitWorkshop Ordner.

```{.bash}
git status

git add README.md

git status

git add Lektionen/Lektion1:Das-erste-Repositorie.md

git status
```

Für eine kürzere Statusausgabe: ``git status -s``, dabei steht ``>A<`` für Added, ``>??<`` für nicht beobachtete Dateien und ``> M<`` ``>M <`` veränderte Datei im und nicht im Statigbereich.

```{.bash}
git add -A # Alles hinzufügen

git commit -m "Mein erster Commit"

git status
```
