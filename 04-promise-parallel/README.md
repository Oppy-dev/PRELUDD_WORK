# Promise Race

The goal is to implement a NodeJS function that returns a promise which resolves (or rejects) when *all* of the given functions (given as its arguments) which all return promises, resolve or reject.

The `parallel` function takes a single argument: a list of Function. All of these functions return a promise.

Do not use already existing NodeJS methods that does the job!

```javascript
    function parallel(functions) {
        // functions is a list of Function that all return a Promise
        // TODO
    }

    parallel([ () => Promise.resolve(12), () => Promise.resolve(13) ]).then(result => console.log(result));
    // Should print "[12,13]"
```