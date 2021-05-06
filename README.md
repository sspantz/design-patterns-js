# Design Patterns

> Examples of Design Patterns with JavaScript

## [Principles of Design Patterns](./principles-of-design-patterns.md)

1. Single Responsibility Principle
1. Open-Closed Principle
1. Liskov Substitution Principle
1. Dependence Inversion Principle
1. Interface Segregation Principle
1. Law Of Demeter
1. Composite/Aggregate Reuse Principle

## Creational Patterns

### Factory

```javascript
class ClothFactory {
  constructor(type) {
    switch(type) {
       case "shirt": return new Shirt();
       case "skirt": return new Skirt();
       case "pants": return new Pants();
       default: throw new Error('No input!')
    }
  }
}

class Shirt {
  constructor() {
    this.showMessage();
  }
  showMessage() {
    console.log("Manufacturing Shirt...");
    setTimeout(() => console.log("Done"), 1000);
  }
}

class Skirt {
  constructor() {
    this.showMessage();
  }
  showMessage() {
    console.log("Manufacturing Skirt...");
    setTimeout(() => console.log("Done"), 1200);
  }
}

class Pants {
  constructor() {
    this.showMessage();
  }
  showMessage() {
    console.log("Manufacturing Pants...");
    setTimeout(() => console.log("Done"), 1500);
  }
}
```


## Structural Patterns

## Behavioural Patterns
