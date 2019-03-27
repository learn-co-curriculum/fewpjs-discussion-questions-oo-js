# OO JS Discussion

## Objectives

* Practice reading and reasoning about code
* Discuss events with out

## Exercise

Take a look at each of the code samples below. For each sample, work with your group to answer the following questions.

1. What does each line of code do?
2. How does this piece of code work?
3. Given this code sample, what can you learn or describe about JavaScript

## Example 1

```javascript
const kanye = {firstName: 'Kanye', lastName: 'West', bestSong: 'Monster'}
kanye.firstName // 'Kanye'
kanye['firstName'] // 'Kanye'

let prop = 'lastName'
kanye.prop // undefined
kanye['prop'] // undefined
kanye[prop] // 'West'
```

## Example 2

```javascript
class Artist {

}

const kanye = new Artist
kanye.bestSong // undefined
kanye.bestSong = 'Gone'
kanye.bestSong // 'Gone'


```

## Example 3

```javascript
class Artist {
  constructor(firstName, lastName, bestSong){
    this.firstName = firstName
    this.lastName  = lastName
    this.bestSong  = bestSong
  }
}

const kanye = new Artist('Kanye', 'West', 'Monster')
kanye.firstName // 'Kanye'
kanye.lastName  // 'West'
kanye.lastName = 'Kardashian-West'
kanye.lastName // 'Kardashian-West'

```

## Example 4

```javascript
class Artist {
  constructor(firstName, lastName, bestSong){
    this.firstName = firstName
    this.lastName  = lastName
    this.bestSong  = bestSong
  }
}

const kanye = new Artist('Kanye', 'West', 'Monster')
kanye.firstName // 'Kanye'
kanye.lastName  // 'West'
kanye.lastName = 'Kardashian-West'
kanye.lastName // 'Kardashian-West'

```

## Example 5

```javascript
class Artist {
  constructor(firstName, lastName, bestSong){
    this.firstName = firstName
    this.lastName  = lastName
    this.bestSong  = bestSong
  }
}

const kanye = new Artist('Monster')
kanye.firstName // 'Monster'
kanye.lastName  // undefined
kanye.bestSong  // undefined

```

## Example 6

```javascript
class Artist {
  constructor({firstName, lastName, bestSong}){
    this.firstName = firstName
    this.lastName  = lastName
    this.bestSong  = bestSong
  }
}

const kanye = new Artist({bestSong: 'Monster', firstName: 'Kanye', lastName: 'West'})
kanye.firstName // 'Kanye'
kanye.lastName  // 'West'
kanye.bestSong  // 'Monster'

```
