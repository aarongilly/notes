---
tags:
- technique
- coding
---
**Index of 10 Design Patterns**

## Creational

**Singleton** - a class with one instance. With a Private constructor. In [[JavaScript]] you can basically just use a global Object instead. In C++, not so much. The [[PDW]] library uses this pattern.

**Prototype** - create an Object. Clone that Object many times.

![Untitled](Untitled%2010.png)

**Builder** - build an instance of a class bit-by-bit chaining method calls that return this. This is actually what I’m doing with Wrapper-Lib. How about that.

**Factory** - build a function that creates specific, often repeated configurations of Class instances. I think I’m *also* doing this with Wrapper-Lib via the “LabeledInput” thing.

## Structural

**Facade** - A Class that sits on other classes (sometimes multiple other classes) and creates a more user-friendly interface. Again, definitely what Wrapper-Lib was doing.

**Proxy** - substituting a placeholder for an object that allows finer-grained access to controls. This allows you to override ‘get’ and ‘set’ and do extra stuff. This looks dope.

```jsx
const original = { name: 'jeff' };

const reactive = new Proxy(original, {
  get(target, key) {
    console.log('Tracking: ', key);
    return target[key];
  },
  set(target, key, value) {
    console.log('updating UI...');
    return Reflect.set(target, key, value);
  },
});

reactive.name; // 'Tracking: name'

reactive.name = 'bob'; // 'updating UI...'
```

## Behavioral

**Iterator** - things like the for loop. In JavaScript, it’s a function that returns a “next()” function.

**Observer** - one-to-many relationship where changes are pushed to subscribers. Wrapper-Lib is using this hard.

**Mediator/Broker** - breaking down many-to-many relationships by inserting a middleman that enables 2 separate many-to-one relationships. Middleware is a mediator. I think my “Binding” Class in Wrapper-Lib is working like that.

**State** - splitting out possible states of class instances, creating a separate class for each possible state, then setting the state of the top class to one of the stateClasses. The logic specific to that state can be held in the state class.

```
interface State {
  think():string;
}

class HappyState implements State {
  think() {
    return 'I am happy 🙂';
  }
}

class SadState implements State {
  think() {
    return 'I am sad 🙁';
  }
}

class Human {
  state:State;

  constructor() {
    this.state = new HappyState();
  }

  changeState(state) {
    this.state = state;
  }

  think() {
    return this.state.think();
  }

}

const human = new Human();
console.log(human.think());
human.changeState(new SadState());
console.log(human.think());
```

## More Research

“Design Patterns” book. Reference by Fireship. 

---

## Source
- [[YouTube]]
- [[Fireship YouTube Channel]]

# Other Sources

[https://fireship.io/lessons/typescript-design-patterns/](https://fireship.io/lessons/typescript-design-patterns/)

[10 Design Patterns Explained in 10 Minutes](https://www.youtube.com/watch?v=tv-_1er1mWI)

### Related Notes
- ...