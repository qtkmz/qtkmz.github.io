---
layout: post
title:  "Scala で Fizz Buzz"
date:   2017-05-29 00:00:00 +0900
categories: 
---

## if-else で

```scala
for (i <- 1 to 15) {
  if (i % 15 == 0)
    print("Fizz Buzz")
  else if (i % 5 == 0)
    print("Buzz")
  else if (i % 3 == 0)
    print("Fizz")
  else
    print(i)
  print(", ")
}
```

## match で

```scala
for (i <- 1 to 15) {
  i match {
  case x if i % 15 == 0 => print("Fizz Buzz")
  case x if i % 5 == 0 => print("Buzz")
  case x if i % 3 == 0 => print("Fizz")
  case _ => print(i)
  }
  print(", ")
}
```

## match とタプルで
```scala
for (i <- 1 to 15) {
  (i % 3, i % 5) match {
  case (0, 0) => print("Fizz Buzz")
  case (_, 0) => print("Buzz")
  case (0, _) => print("Fizz")
  case _ => print(i)
  }
  print(", ")
}
```
