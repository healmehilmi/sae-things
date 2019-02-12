# Pseudoelemente

## Allgemeines

Pseudoelemente wirken sich auf Elemente so aus, als ob sie zusätzliche Elemente in das Markup einfügen würden, um Styling auf Teile des Elements anwenden zu können, die sonst ohne zusätzliches Markup nicht ansprechbar/selektierbar wären.

In CSS3 wurde eine neue Schreibweise vorgestellt, um Pseudoelemente besser von Pseudoklassen differenzieren zu können. Dabei werden Pseudoelemente mit zwei Doppelpunkten geschrieben. Diese Schreibweise funktioniert nicht <=IE8

```
p::first-line { 

}
```

## CSS 2.1 Pseudoelemente

Liste der CSS 2.1 Pseudoelemente: http://www.w3.org/TR/CSS21/selector.html#pseudo-element-selectors

Liste der CSS 3 Pseudoelemente: http://www.w3.org/TR/css3-selectors/

### Spricht den ersten Buchstaben an

```
p:first-letter { }
```

### Spricht die erste Zeile an

```
p:first-line { }
```

### Fügt Inhalt direkt nach dem Starttag hinzu

```
:before { }
```

### Fügt Inhalt direkt vor dem Endtag hinzu

```
:after { }
```
