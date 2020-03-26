# [24 March 2020]

## Web API & Promises -- Microtask Queue

1. priority</br>

```javascript
process.nextTick > promise.then > setTimeout > setImmediate
//microtask queue over the Callback queue (all global code run)
```

# [25 March 2020]

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
//Using the prototype property allows us to add new properties to object constructors
userCreator.prototype.increment = function(){
    this.score++;
}

const user1 = new userCreator("will",10)

```

# [26 March 2020]
## Deep JS
1. NaN is the only value that not equals to itself.
2. Don't use <span color= "#00BFFF">new<span>:<br>
   a. String()<br>
   b. Number()<br>
   c. Boolean()
3. 