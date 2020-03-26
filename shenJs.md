# [24 March 2020]

## Web API & Promises -- Microtask Queue

1. priority</br>

```javascript
process.nextTick > promise.then > setTimeout > setImmediate
//microtask queue over the Callback queue (all global code run)
```

## Class & OOP -- Factory functions
1. Different ways to create an object
2. Javascript: prototypal feature
3. Functions are both objects and functions

```javascript
function userCreator(name,score){
    this.name = name;
    this.score = score;
}
//you can not add a new property to an existing object constructor
//
userCreator.prototype.increment = function(){
    this.score++;
}

const user1 = new userCreator("will",10)

```