# Hintergrund

## background-color (Hintergrundfarbe)

Die Hintergrundfarbe eines Elements definieren. Der Standardwert ist transparent (Durchsichtig). Farbwerte könnnen hexadezimal, mit Schlüsselwörtern, in rgb() oder rgba()-Werten angegeben werden.

```
body {
  background-color: #ff0;
}
```

## background-image (Hintergrundbild)

Das Hintergrundbild eines Element festlegen. Dieses wird standardmäßig links oben eingebunden und in x- und y-Richtung wiederholt.

```
body {
  background-image:url('pfad/zur/hintergrundgrafik.jpg); 
}
```

## background-repeat (Wiederholung)

Festlegen ob und wie sich ein Hintergrundbild wiederholt.

**repeat (Standartwert)**: Das Hintergrundbild wird vertikal und horizontal wiederholt

**no-repeat**: Das Hintergrundbild wird nicht wiederholt

**repeat-x**: Das Hintergrundbild wird nur horizontal wiederholt

**repeat-y**: Das Hintergrundbild wird nur vertikal wiederholt

```
body { 
    background-image:url('pfad/zur/hintergrundgrafik.jpg);
    background-repeat:repeat-x; 
}
```

## background-position (Positionierung)

Festlegen an welcher Stelle das Hintergrundbild beginnt. Dabei kann die horizontale und vertikale Position definiert werden. Standardmäßig ist das Bild in der oberen linken Ecke des Elements positioniert.

### Zahl- und Prozentwerte

Mit Zahl- oder Prozentwerten kann der Abstand der Position zum linken oberen Eck angegeben werden. Zahl- und Prozentwerte können gemischt werden und dürfen auch negativ sein. Der erste Werte entspricht der horizontale Verrückung und der zweite Wert der vertikalen. Wird nur ein Wert angegeben, wird dieser als horizontaler Wert interpretiert und der vertikale Wert ist automatisch 50%.

```
body { 
    background-image:url('pfad/zur/hintergrundgrafik.jpg);
    background-position: 100px 40%;
}
```

### Schlüsselwörter

Die Position des Hintergrundbildes kann auch mit Schlüsselwörtern angegeben werden. Dabei muss für beide Richtungen jeweils ein Schlüsselwort angegeben werden (left - center - right und top - center - bottom).

```
body { 
    background-image:url('pfad/zur/hintergrundgrafik.jpg);
    background-position: right bottom;
}
```

## background (Kurzschreibweise)

Alle Hintergrundeigenschaften lassen sich in einer Zeile zusammenfassen. Wird eine Eigenschaft nicht angegeben, wird ihr Standardwert genommen.

background-color / background-image / background-repeat / background-attachment / background-position

```
body { 
    background: #FF0000 url('hintergrundgrafik.jpg') repeat-x fixed left center; 
}
```


## background-size

Größe des Hintergrundbilds.

```
body {
  background-size: 400px 250px;
}
```

**Numerische Werte (px, em, %, etc..)**: 1-2 Parameter. Erster Wert Breite, zweiter Wert Höhe (optional)

**cover**: Proportionen bleiben erhalten, Bild füllt Element aus und wird wenn nötig abgeschnitten

**contain**: Proportionen bleiben erhalten, Bild füllt Element aus, wenn möglich. Wenn nicht, wird auch nicht abgeschnitten

## background-origin

Gibt an woran sich das Hintergrundbild bei der Positionierung orientieren soll.

```
div {
  background-origin: content-box;
}
```

**content-box**: Relativ zu Inhalt  
**padding-box**: Relativ zum padding (Default)  
**border-box**: Relativ zum border

## background-clip

Gibt an bis wohin die Hintergrundfarbe reicht.

```
section {
  background-clip: padding-box;
}
```

**border-box**: Bis zum äußeren Rand (default)  
**padding-box**: Bis zum border  
**content-box**: Bis zum padding
