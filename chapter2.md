---
  title: "Grundlagen"
  description: "In diesem Kapitel geht es um grundlegende Begriffe, statistische Messgrößen, andere Kennzahlen und den Umgang mit Datensätzen. Dies ist also der Einstieg in die deskriptive Statistik."
  v2: true

---
## Erhebungsart

```yaml
type: PureMultipleChoiceExercise

xp: 50

key: 184223ca51



```

Bob ist ein ganz gewöhnlicher Student. Das neue Semester hat begonnen und heute ist sein erster Tag als Hilfskraft von Herrn Professor Ratistikus. "Was für eine langweilige Aufgabe!", denkt Bob, als er seine erste Aufgabe des Tages erfährt. Der Professor hat ihn gebeten die Teilnehmer seiner Seminare zu zählen. Um welche Erhebungsart handelt es sich dabei?


`@hint`
Bob sieht in jedem Raum nach und zählt die Studierenden. Ein Experiment findet nur bei zwei verschiedenen Bedingungen statt.





`@possible_answers`
- Experiment
- Befragung
- [Beobachtung]

`@feedbacks`
- Das ist leider nicht richtig.
- Das ist leider nicht richtig.
- Herzlichen Glückwunsch!





---
## CSV einlesen

```yaml
type: NormalExercise

xp: 100

key: f3db946150



```

Bob war fleißig und hat in allen Vorlesungen und Seminaren von Prof. Ratistikus die Studierenden gezählt. Er möchte diese Daten mit R auswerten. Dazu möchte er seine csv-Datei namens 'Studierendenzaehlung.csv' unter dem Variablennamen 'Studis' in R laden. Schau dir die Datei vorher gut an.

`@instructions`
Was muss er dazu eingeben? Lese die csv-Datei namens 'Studierendenzaehlung.csv' ein und weise sie dem Variablennamen 'Studis' zu.

`@hint`
Hilfe zu den Funktionen bekommst du mit `help('Funktionsname')`. Hier wird `read.csv2` benötigt und du musst wissen, wie die Variablenzuweisung funktioniert. Beachte auch die Angaben für den Delimiter. Die erste Überschrift ist zu ignorieren. Beachte auch, dass das Arbeitsverzeichnis stimmig sein muss, sonst wird die Datei nicht gefunden.



`@solution`
```{r}
Studis <- read.csv2("Studierendenzaehlung.csv",sep=",",skip=1)
```
`@sct`
```{r}
#test_error()
#test_object("Studis",
#            undefined_msg = "Make sure to define `Studis`!",
#            incorrect_msg = "Have you correctly assigned Studis!")
#success_msg("Awesome! It's considered good style to write spaces either side of the assignment arrow.")
```




