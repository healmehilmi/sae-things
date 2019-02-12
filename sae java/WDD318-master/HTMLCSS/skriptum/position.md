# Position

## position:static

Elemente werden genauso angezeigt, wie im HTML-Code angegeben. Alle Elemente sind standardmäßig `static` positioniert, was bedeutet, dass diese Eigenschaft nicht dezidiert gesetzt werden muss. `left`, `right`, `top` und `bottom` haben bei static positionierten Elementen keine Wirkung.

## position:relative

Ein relativ positioniertes Element wird ausgehend seiner Anfangsposition, entsprechend seiner `top`, `right`, `bottom` oder `left` Werte, verschoben. Zur Positionierung verwendet man entweder `top` oder `bottom` und `right` oder `left`. Verwendet man top und `bottom`, wird `bottom` ignoriert. Verwendet man `left` und `right`, wird `right` ignoriert.

```
div {
  position:relative;
  left:15px;
  top:10px;
}
```

Die Positionierung beeinflusst andere Elemente nicht, dementsprechend kann es sein, dass relativ positionierte Elemente andere überlagern. Nachfolgende Elemente verhalten sich so als ob sich das Element noch immer an seiner ursprünglichen Stelle befindet, das heisst die veränderte Position wird nicht berücksichtigt.

## position:absolute

Absolut positionierte Elemente werden in ihrer Position nicht von vorhergehenden Elementen beinflusst und beeinflussen auch nicht nachkommende. Sie schweben quasi über allen anderen relativ oder statisch positionierten Elementen. Sie werden aus dem Elementfluss herausgerissen und relativ zum nächstgelegenen Elternelement, das `absolut`, `relativ` oder `fixed` positioniert wurde, positioniert. Gibt es ein solches Element nicht, wird vom Wurzelelement (html) ausgegangen.

```
div {
  position:absolute;
  right:20px;
  bottom:0;
}
```

Die Positionierung mit absoluten Werten scheint auf den ersten Blick sehr praktisch zu sein, da sie sehr verständlich ist. Sie kann aber Schwierigkeiten mit sich bringen, da beispielsweise die Möglichkeit besteht, dass sich gewisse Elemente überlagern oder vielleicht gar nicht mehr angezeigt werden, weil sie außerhalb des sichtbaren Bildschirmbereichs sind.

Außerdem sind absolut positionierte Elemente sehr aufwendig zu warten, da man unter Umständen jedes absolut positionierte Element einzeln anpassen muss, sobald sich Änderungen in der Breite, Höhe oder Position eines Elements ergeben.

**Deswegen eignet sich absolute Positionierung nicht fürs Layouting.**

## position: fixed

`position:fixed` funktioniert ähnlich wie `position:absolute`. Der Unterschied liegt aber darin, dass das fixed positionierte Element immer bezogen auf das Browserfenster positioniert wird und dass es sich nicht mitbewegt, wenn die Website gescrollt wird, sondern immer fix auf seiner Position bleibt.

## position: sticky

Elemente mit `position: sticky` behalten ihre Position im Elementfluss, bis sie das obere oder untere Seitenende erreichen und dort „kleben“ bleiben.

```
div {
  position:sticky;
  left: 0;
  top: 100px;
}
```

## z-index

Positioniert man mehrere Elemente, deren Anzeigebereiche sich überlappen, werden die Elemente normalerweise in der Reihenfolge übereinander angezeigt, in der sie definiert wurden. Im Quelltext später vorkommende Elemente überdecken vorhergehende.

Die Reihenfolge kann verändert werden, indem man den Elementen die Eigenschaft `z-index` gibt. Je höher der Wert desto weiter oben das Element.

```
div {
  position:absolute;
  z-index: 500;
}
```

Maximaler z-index: 2147483647 bzw. 16777271 (webkit)

Die Stapelung wirkt nicht bei statisch positionierten Elementen. Statisch positionierte Elemente der selben Ordnungsebene liegen immer unter `relativ`, `absolute` oder `fixed` positionierten Elementen.

Die Stapelung bezieht immer auf Elemente der selben Ordnungsebene.
