# Settings
| Befehl | Bedeutung |
| ------ | --------- |
| ``git config --global color.ui true`` | Aktiviert eine farbige Ausgabe auf der Konsole. |
| ``git config --global user.name "Max Muster"`` | Setzt einen Nutzernamen der in der Historie verwendet wird |
| ``git config --global user.email mail@adresse.com`` | Setzt die E-Mail des Nutzers |
| ``git config --global core.editor vim`` | Setze den commit Editor |
| ``git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -nosession"`` | Für Windowsnutzer |
| ``git config --global rebase.autosquash true`` | Führt bei ``git rebase`` automatisch ``git rebase --autosquash`` durch |
| ``git config --global pull.rebase true`` | Führt automatisch ``git pull --rebase`` aus wenn ``git pull`` ausgeführt wird. |


# Initial
```
git init
git clone <Remote> <LocalFolder>
```
# Informationen
```
git show - den letzten Commit in vollem Umfang anschauen
git log - die gesammte Versionsgeschichte anzeigen
git diff - die Änderungen vom letzten Commit zum aktuellen Stand anzeigen
gitk - Visualisierung der Repositories
tig - Visualisierung in Textform
```
# Branches
```
git branch - auflisten aller Branches
git branch <branchname> - erzeugt einen neuen Branch
git checkout <branchname> - wechseln in einen Branch
git branch -d <branchname> [<branchname2>] - löschen eines oder mehrerer Branches
```
# Commit
```
git add - Änderungen zum Stack hinzufügen
git commit -m <massage> - Commit inkl. Commitmassage
```
# Merge
```
git rebase <branchname> - bringt den HEAD auf den stand des angegebenen Branches
git merge <branchname> [<branchname2>] - merged den angegeben Branch in HEAD [in den angegeben Branch]
```
# Rückgängig machen
```
git reverte <commit> - Erstellt einen neuen commit der eine alte änderung Rückgängig macht
git reset HEAD - Setzt den Index zurück
git checkout HEAD~2 - Stellt den zustand vor zwei Commits wieder her
git show HEAD~2:<datei> - anschauen wie eine Datei vor zwei Versionen aussah
git reset --hard HEAD~2 - Löscht die letzten beiden Commits unwiederruflisch!
```
