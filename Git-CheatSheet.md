# Git / Github Cheatsheet

## Inhaltsverzeichnis

- [Git / Github Cheatsheet](#git--github-cheatsheet)
  - [Inhaltsverzeichnis](#inhaltsverzeichnis)
  - [Einleitung](#einleitung)
  - [Git Storage Model](#git-storage-model)
  - [Repository erstellen](#repository-erstellen)
  - [Index Commands](#index-commands)
    - [Stage Commands](#stage-commands)
  - [lokales Repository Commands](#lokales-repository-commands)
  - [Remote Repository Commands](#remote-repository-commands)

#

## Einleitung
Dies ist mein Cheat-Sheet über Git. Dieses Cheat-Sheet ist in Markdown geschrieben.

## Git Storage Model
![Mödel](/Git_StorageDataFlow1.png)

## Repository erstellen
Repo initialisieren

`$ git init`

## Index Commands
File Status ausgeben

`$ git status`

Neues / geändertes File dem Index hinzufügen

`$ git add {file}`

`$ git add .` (Alles hinzufügen)

File aus dem Index entfernen

`$ git reset HEAD {file}`

### Stage Commands
Zeigt was im Worsplace geändert, aber noch nicht im Index (staged) ist

`$ git diff`

Zeigt was bereits zum Commit vorgemerkt wurde

`$ git diff --cached`

## lokales Repository Commands
Änderungen vom Index in das lokale Repository übertragen

`$ git commit -m "(Description)" {file}`

History vom Commit ansehen

`$ git log`

## Remote Repository Commands
Verknüpftes Remote Repository anzeigen

`$ git remote -v`

Alle Änderungen vom remote Repo in den Workplace herunterladen

`$ git pull`

Alle Änderungen vom lokalen Repo in das remote Repo hochladen

`$ git push origin`

Remote Repo hinzufügen

`$ git remote add origin git@github.com:youraccount/test.git`