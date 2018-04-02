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
```

Nun sollte bei allen die Git frisch installiert haben eine Fehlermeldung auftauchen. Git benötigt für den Commit einen Benutzernamen und eine E-Mail Adresse um diese in der Commithistory anzeigen zu können.

```{.bash}
git commit -m "Mein erster Commit"

git status
```

## Git Configuration

```
# Config in Yaml file
cat ~/.gitconfig # Zeigt die globalen Konfigurationen von Git

cat .git/config

git config user.name # Wirkt sich auf das Repository aus

git config --global user.name # Wirkt sich auf die globale Konfiguration aus.
```


## Die History

Mit hilfe von ``git log`` können wir uns nun die History anzeigen lassen.
bekommen
```{.bash}
commit a4045440894fbcf790782a41469016f3f84acc57 (HEAD -> master)
Author: Kreativmonkey <kreativmonkey@ffmyk.de>
Date:   Sun Feb 18 14:09:49 2018 +0100

    Mein erster Commit
```

| Reverenzierung | Beschreibung |
| -------------- | ------------ |
| commit-id (kurz - lang) | Sie ist eine SHA-1-Checksumme, sie ist eindeutig und wird zur genauen Identifizierung eines Commits benötigt. |
| HEAD | Aktueller stand |
| master | Branch |

