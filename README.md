# adigrams

Draw boxes in ascii...

```
$ cat logo
  +------------+
  | ADIGRAMS   |
  |        +---+------+
  |        | 4 |      |
  +--------+---+      |
           |    LYFE  |
           +----------+
```

...and turn them into Unicode:

```
$ adigrams < logo
  ┌────────────┐
  │ ADIGRAMS   │
  │        ┌───┼──────┐
  │        │ 4 │      │
  └────────┼───┘      │
           │    LYFE  │
           └──────────┘
```

## Examples

### Lines

Lines must occupy two adjacent chars:

```
--- horizontal |
      vertical |
  - minus
    pipe |
```

```
─── horizontal │
      vertical │
  - minus
    pipe |
```


### Line Style

Different characters produce different line thickness:

```
reg thk dbl
--- ___ ===

 |   !   H
 |   !   H

```

```
reg thk dbl
─── ━━━ ═══

 │   ┃   ║
 │   ┃   ║

```


### Boxes

Box corners can be either square (`+`) or rounded (`*`):

```
+---+  +___+  +===+  +===+  *---*
|reg|  !thk!  HdblH  !lol|  |crv|
+---+  +___+  +===+  +---+  *---*
```

```
┌───┐  ┏━━━┓  ╔═══╗  ?═══╕  ╭───╮
│reg│  ┃thk┃  ║dbl║  ┃lol│  │crv│
└───┘  ┗━━━┛  ╚═══╝  ┖───┘  ╰───╯
```

Not all combinations of line thickness are available with the standard Unicode
box drawing characters.

For curved corners, only the regular line thickness is available.
