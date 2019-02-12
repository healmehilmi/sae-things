# Sonstiges

## border-radius

Mit border-radius kann man die Ecken eines Elements abrunden.

[Live-Beispiele](https://codepen.io/matuzo/pen/yYabeK?editors=110)

### Ein Wert für alle Seiten

```
div {
  border-radius: 20px;
}
```

### Zwei Werte

top-left und bottom-right / top-right und bottom-left

```
div {
  border-radius: 20px 10px;
}
```

### Drei Werte

top-left / top-right und bottom-left / bottom-right

```
div {
  border-radius: 20px 40px 10px;
}
```

### Vier Werte

top-left / top-right / bottom-right / bottom-left

```
div {
  border-radius: 20px 40px 10px 5px;
}
```

### Jede Seite einzeln

```
div {
  border-top-left-radius: 20px;
  border-top-right-radius: 40px;
  border-bottom-right-radius: 10px;
  border-bottom-left-radius: 5px;
}
```

### Unterschiedliche Radien horizontal und vertikal

```
div {
  border-radius: 20px/50px;
}
```

```
div {
  border-radius: 20px 30px 10px 8px/ 90px 5px 50px 20px;
}
```

### Kreise und Ellipsen

Man kann auch Prozentwerte angeben. Das ist speziell sehr brauchbar, wenn man Kreise und Ellipsen erzeugen will.

```
div {
  border-radius: 50%;
}
```

## Vendorprefixes

Solange Browser den Einsatz neuer Eigenschaften testeten und noch nicht fix in ihr Repertoire aufgenommen haben, haben sie sogenannte Browserprefixe (vendor prefixes) eingesetzt.

Beispielsweise: "-webkit-text-stroke: 10px" wird nur von Webkitbasierenden Browsern erkannt

Sobald die Definition der Eigenschaft final war und die Browser die technische Umsetzung abgeschlossen hatten, wurde die Eigenschaft in das offzielle Eigenschaftenset des Browsers aufgenommen.
Alle Browserversionen ab diesem Zeitpunkt setzen den Prefix nicht mehr voraus, ältere natürlich immer noch.

Folgende Prefixe sind relevant:

    `-o-eigenschaft` - Opera
    `-ms-eigenschaft` - IE
    `-webkit-eigenschaft` - Webkit/Chrome/Safari
    `-moz-eigenschaft` - Firefox

Neue Browserversionen verwenden keine Prefixe mehr. Stattdessen muss man experimentelle Features im Browser aktivieren.

## box-shadow

Schatten in oder um ein Element

```
body {
  box-shadow: 10px 10px 10px 5px #f00 inset;
}
```

`box-shadow`: [horizontaler Versatz][vertikaler versatz] [Kantenhärte (optional)][ausbreitung (optional)] [Farbe (optional)];

Zusätzlich kann auch noch der Wert inset vergeben werden, wenn es ein innerer Schatten werden soll.

Es können einem Element auch mehrere Schatten zugewiesen werden.

```
body {
  box-shadow: -10px -10px #f00, 10px 10px #00f;
}
```

## Favicons

Generator: <https://realfavicongenerator.net/>

## Frontend Checklist

Frontend best practices: <https://github.com/thedaviddias/Front-End-Checklist>

## Animation

<https://css-tricks.com/almanac/properties/a/animation/>
