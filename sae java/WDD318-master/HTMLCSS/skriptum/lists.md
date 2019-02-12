# Listen

## list-style-type (Art des Aufzählungszeichens)

Mit list-style-type wird die Art des Aufzählungszeichens bzw. der Nummerierung festgelegt.

```
ul {
  list-style-type: decimal-leading-zero;
}
```

**none**: Kein Aufzählungszeichen

**circle**: Kreise

**disc**: Gefüllte Kreise (Standardwert)

**square**: Quadrate

**decimal**: Dezimal

**decimal-leading-zero**: Dezimal mit 0 davor

**lower-alpha**: Kleine Buchstaben

**upper-alpha**: Große Buchstaben

**lower-roman**: Kleine römische Ziffern

**upper-roman**: Große römische Ziffern


## list-style-image (Eigenes Aufzählungszeichen)

Mit `list-style-image` kann man eigene Aufzählungszeichen definieren

```
ul { 
    list-style-image: url('zeichen.jpg');
}
```

## list-style-position (Positionierung des Aufzählungszeichens)

`list-style-position` gibt ab ob die Aufzählungszeichen innerhalb oder außerhalb des Textblocks positioniert sind.

```
ul { 
  list-style-position: outside;
}
```

**outside (Standardwert)**: Aufzählungszeichen außerhalb des Textblockes

**inside**: Aufzählungszeichen innerhalb des Textblockes

## list-style (Kurzschreibweise)

Kurzschreibweise für die Formatierung von Listen. Wird kein Wert angegeben, wird der jeweilige Standardwert genommen.

`list-style-type / list-style-position / url (‘’)`

```
ul { 
    list-style: outside url('zeichen.gif');
}
 
ol { 
    list-style: lower-greek inside; 
}
```

