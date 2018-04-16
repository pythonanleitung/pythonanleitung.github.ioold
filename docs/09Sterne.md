# Sterne zeichnen mit Turtle

> ### Übung
> Zeichnen Sie einen Fünfstern. Der Innenwinkel in einem Fünfstern ist 35° Grad.

Im Folgenden wird es Ziel sein viele Fünfsterne zu zeichnen in unterschiedlichen Größen.
Eine Möglichkeit das zu tun wäre nun, den bisher geschriebenen Code einfach zu kopieren und woanders wieder einzufügen.
Man muss nun nur noch ein paar Zahlen ändern und fertig ist der zweite Stern.

Beim Programmieren möchte man aber solche wiederholende Aufgaben eigentlich lieber den Computer selbst machen lassen.
Das heißt man schreibt zunächst eine Schablone und sagt dem Computer was er veränderbar in dieser Schablone machen soll.

Eine Schablone, beim Programmieren nennt man solche Schablonen Funktion, erstellt man So:

```python
def stern(größe):
    t.forward(größe)
    t.left(36)
```

Indem man zunächst das Schlüsselwort `def` schreibt, sagt man Python dass nun eine Schablone kommt, die nicht sofort ausgeführt
werden soll, sondern die sich das Programm erstmal merken soll. Danach folgt ein beliebiger Name in diesem Fall ist `stern` gewählt worden.
Zuletzt kommt in Klammern eine Liste der veränderlichen Namen als Platzhalter. Für den Stern wird erstmal nur die `größe` veränderlich sein.
Statt nun eine feste Zahl vorwärts zu gehen, muss man jetzt die veränderliche größe aus der Schablone vorwärts gehen.
Für alle Fünfsterne sind die Winkel die selben. Das heißt man kann die Zeilen mit `left` unveränderbar lassen,
indem man einfach konstante Zahlen schreibt.

Diese Funktionsschablone wird jetzt aber noch nicht ausgeführt. Man sagt Python nur wie die Schablone aussieht.
Um jetzt einen Stern zu zeichnen, muss man diese Schablone verwenden, und Python sagen, welcher Platzhalter welchen Wert annehmen soll.

```python
stern(größe=100)
```

Jetzt wird tatsächlich etwas gezeichnet natürlich noch nicht der volle Stern, da bis jetzt nur eine Linie gezeichnet wird.
Zunächst schreibt man also einfach den Namen der Funktion,
dann in Klammern die Zuweisungen, welcher Platzhalter welchen Wert erhalten soll. Es kann Ihnen hier auffallen,
dass Sie die ganze Zeit schon solche Funktionen verwendet haben zum Beispiel `print`, `input`, ….

> ### Übung
> 1. Ergänzen Sie die `stern`-Funktion, sodass sie den gesamten Stern zeichnet
> 2. Zeichnen Sie mehrere verschieden große Sterne.