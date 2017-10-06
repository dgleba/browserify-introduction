# browserify-introduction
[Introduction to browserify using Scotch.io tutorial](https://scotch.io/tutorials/getting-started-with-browserify)

> Use Case;

Browserify delves into the dependency file to make an independent individual list of each file required.

There are other uses as well.

```
browserify main.js -o bundle.js
```

#### Source Maps
To isolate the bugs
```browserify --debug main.js -o bundle.js```

To seperate bundle and map info
```npm install --global exorcist```

```browserify main.js --debug | exorcist bundle.map.js > bundle.js```

This rips all the source map information out of bundle.js and spits it into bundle.map.js instead.
