# Pseudoklassen

Liste der CSS 2.1 Pseudoklassen: <http://www.w3.org/TR/CSS21/selector.html#pattern-matching>

Liste der CSS 3 Pseudoklassen: <http://www.w3.org/TR/css3-selectors/#selectors>

## Für Verweise zu noch nicht besuchten Seiten

```
a:link { }
```

## Für Verweise zu bereits besuchten Seiten

```
a:visited { }
```

Wichtig: [Limitiertes Styling für :visited](https://hacks.mozilla.org/2010/03/privacy-related-changes-coming-to-css-vistited/)  

## Befindet man sich mit der Maus über einem Element

```
:hover { }
```

## Für aktive Elemente (bspw. ein Link der gerade geklickt wird)

```
:active { }
```

## Für fokusierte Elemente (bspw. ein Formularfeld)

```
:focus { }
```

## Ein Element, das das erste Kindelement eines anderen Elements ist

```
:first-child { }
```

## Ein Element, das das letzte Kindelement eines anderen Elements ist

```
:last-child { }
```

## Ein Element basierend auf der Sprache selektieren.

Die Sprache muss nicht explizit für dieses Element mittels lang-Attribut definiert werden. Es kann die Sprachdeklaration von einem Elternelement erben.

```
:lang() { }
```

## nth-child

Ausgehend vom ersten Element wird das n-te Element selektiert.

### Das zweite Kindelement selektieren
```
li:nth-child(2) {
  color: red;
}
```

### Jedes dritte Kindelement selektieren

```
li:nth-child(3n) {
    color: blue;
}
```

### Jedes zweite Kindelement beginnend beim dritten selektieren

```
li:nth-child(2n+3) {
    background: #000;
}
```

## nth-last-child

### Ausgehend vom letzten Element wird das n-te Element selektiert.
```
li:nth-last-child(4) {
    border: 10px solid red;
}
```

`nth-last-child` kann genauso angewendet werden wie `nth-child`
