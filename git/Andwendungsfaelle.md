# Anwendungsfälle
<br><br>
### Erstellen eines Projekts
#### Ein existierendes Verzeichnis als Git Repository initialisieren

```
git init
```
oder Git-Repo auf https://github.com/ erstellen


#### Leeres Projekt aus Git-Repo clonen


```
git remote add origin https://github.com/htl-leonding/my-project.git
git push -u origin master
```

#### Bereits bestehendes Projekt ins Git-Repo commiten

```
echo "# delete-me-please" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/htl-leonding/my-project.git
git push -u origin master
```
<br>
<br>

### Ein Projekt aus dem Repos downloaden (clonen)

```
git clone https://github.com/davidandraschko/GitBefehle.git
```
oder als .zip auf https://github.com/ downloaden

<br><br>

### Neue und/oder geänderte Dateien ins das Repo einpflegen

#### Dateien in die Staging Area einpflegen


##### Alle geänderten Dateien in Staging Area einpflegen

```
git add .
```

##### Bestimmte Datei in Staging Area einpflegen

```
git add dateiname.md
```

<br>

#### Dateien aus der Staging Area entfernen

##### Alle Dateien die mit add hinzugefügt wurden aus Staging Area entfernen

```
git reset HEAD .
```

##### Bestimmte Datei aus Staging Area entfernen

```
git reset HEAD dateiname.md
```
<br>

#### Dateien in das local-repo einpflegen

```
git commit -m "Commit Message"
```

<br>

#### Dateien aus dem local-repo entfernen

```
git reset --soft HEAD^
```

<br>

#### Dateien in das remote-repo einpflegen

```
git push origin master
```

<br>

#### Dateien aus dem remote-repo entfernen

```
git push -f origin HEAD^:master
```

<br>
<br>

### Status des Git-Working-Directories ansehen

```
git status
```

<br>
<br>

### Pretty Printing für Git-Logs

<https://stackoverflow.com/questions/1057564/pretty-git-branch-graphs>

ev. mit Verwendung von .gitconfig

<br><br>


### Zweige für eigene Features erstellen

```
git checkout -b TestBranch1
git push origin Testbranch1
```

<br>

### Branch wechseln

```
git checkout TestBranch2
```

<br>

### Branch mergen

```
git merge BranchName
```

<br><br>

### Pull requests durchführen

#### Auf https://github.com/ im Repo unter den Branches einen Pull Request durchführen
- Jemand besitzt ein Repo
- Ein anderer cloned dieses Repo und möchte etwas im Original Repo ändern
- Er/Sie führt einen Pull Request durch
