# [24 March 2020]

## Web API & Promises -- Microtask Queue

1. priority</br>

```javascript
process.nextTick > promise.then > setTimeout > setImmediate
//microtask queue over the Callback queue (all global code run)
```

## Class & OOP -- Factory function