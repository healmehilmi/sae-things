# Selektoren

## Tag-Selektor

```
h1 {

}
````

## Class-Selektor

```
.heading {

}
````

## id-Selektor

```
#site-heading {

}
````

## Attribut-Selektor

### Elemente mit einem `title` Attribut.
```
[title] {

}
````

###Elemente mit einem `type` Attribut mit dem Wert "text".

```
[type="text"] {

}
````

###Link mit einem `title` Attribut.

```
a[title] {

}
````

### E[foo~="bar"]

bar kommt im Attributwert als eigenständiges Wort vor

```
a[title="~wort"] {

}
````

### E[foo*="bar"]

bar kommt im Attributwert egal wie und wo vor

### E[foo^="bar"]

Attributwert beginnt mit “bar"

### E[foo$="bar"]

Attributwert endet mit “bar”

```
[href$=".html"] {
    text-decoration: none;
}
```
