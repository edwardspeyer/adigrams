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

Lines must occupy two adjacent chars

```
--- horizontal line

|   vertical line
|

-   an actual minus
|   an actual pipe
```

```
─── horizontal line

│   vertical line
│

-   an actual minus
|   an actual pipe
```
