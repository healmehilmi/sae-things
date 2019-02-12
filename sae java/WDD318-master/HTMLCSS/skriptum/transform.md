# transform

Visuelle Manipulation eines Elements.

## Skalieren

x-fach skalieren.

```
.element {
  transform: scale(20);
}
```

oder auch nur einzelne Seiten.

```
.element {
  transform: scale(2, 3);
  transform: scaleX(2); 
  transform: scaleY(.5);
}
```

## Schräg stellen

```
.element {
  transform: skewX(25deg);
  transform: skewY(25deg);
}
```

## Rotieren

```
.element {
  transform: rotate(25deg);
}
```


Oder auch

```
.element {
  transform: rotateY(25deg);
  transform: rotateX(25deg);
  transform: rotateZ(25deg);
}
```

## Bewegen

```
.element {
  transform: translate(20px, 10px);
}
```

oder auch


```
.element {
  transform: translateX(value);
  transform: translateY(value);
}
```

## Mehrere Werte

```
.element {
  transform: scale(20) skew(-20deg);
}
```


[Mehr über transforms](https://css-tricks.com/almanac/properties/t/transform/)
