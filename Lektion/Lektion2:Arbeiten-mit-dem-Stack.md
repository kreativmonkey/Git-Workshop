# Arbeiten mit dem Stack

* Was ist der Stack

## Neue Version

Wir ändern die ``Lektion/Lektion2:Arbeiten-mit-dem-Stack.md`` Datei und entfernen diese Zeile.

```{.bash}
git status

git diff

git add Lektion/Lektion2:Arbeiten-mit-dem-Stack.md # Tab vervollständigen!

git commit -m "Überflüssige Zeile entfernt"

git log
```

> Für eine divitilere auswahl der hinzuzufügenden Zeilen einer Datei kann man mit ``git add -p`` nur einzelne parts hinzufügen.

> Da ``git diff`` nur die Änderungen zwischen dem aktuellen Ordner und dem letzten Commit ohne den Dateien im Stagingbereich anzeigt, gibt es noch die befehle ``git diff --staged`` und ``git diff --cached``.

## Mehrere Änderungen in einem Commit

Wir ändern die ``index.html`` und die README Datei.

```{.bash}
git status

git commit -a -m "Namensgebung"
```

Die Größe von Commmits sollten immer nur so klein wie möglich und so groß wie nötig sein. Wenn Sie in Projekten wie dieser statischen Webseite arbeiten, dann sollten Sie zum Beispiel Inhalte auf Unterseiten nur dann in einen Commit zusammenfassen, wenn diese strikt zusammengehören! Das Stichwort ist "Logische Änderungen".


## Änderungen aus dem Stagingbereich nehmen

Wir ändern wieder einmal die ``index.html``.

```{.bash}
git add index.html

git reset HEAD index.html

git checkout -- index.html # änderungen rückgängig machen!
```

HEAD = der HEAD ist immer der aktuelle Stand des branches in dem man sich befindet.
