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
2. Don't use <span style = "color: #00BFFF">new<span>:<br>
   a. String()<br>
   b. Number()<br>
   c. Boolean()
3. Understand the usage of if(!!expression)
   ```javascript
   if(!!last)
   //explain: 
   //if last: null or undefined => !last =true;
   //!!last => false;
   //therefore, !!last returns the real boolean
   ```
4. Coercion: corner cases
   ```javascript
   1 < 2 < 3  // true
   3 > 2 > 1  //false
   //explain:
   // 1 < 2 => TRUE(1)
   //1<3  TURE 
   ```

# [08 April 2020]

## Vue.js

1. **Qeustion**: Vue npm run serve starts on random port <br>
   **Solution**: open package.json file, add portfinders and run `npm install` afterwards.
   ```json
   "resolutions": {
      "@vue/cli-service/portfinder": "1.0.21"
    }
    ```
2. Lifestyle hooks:
   <li>  'beforeCreate'</li>
   <li>'created'</li>
   <li>'beforeMount'</li>
   <li>'mounted'</li>
   <li>'beforeUpdate'</li>
   <li>'updated'</li>
   <li>'beforeDestroy'</li>
   <li>'destroyed'</li>
   <li>'activated'</li>
   <li>'deactivated'</li>
   <li>'errorCaptured'<li>
3. 