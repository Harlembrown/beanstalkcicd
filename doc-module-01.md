## Lab 1 : Create a sample Node REST API

In this module, we create a simple Node REST API with Express test it locally on our Cloud9 environment.

### 1. Create Node REST API

#### 1.1 Download sources

1.  Run this command to download source files for this Lab

```
$ git clone https://github.com/fabianleeaws/beanstalkcicd.git
```

#### 1.2 Copy sample Node code over to current directory

1.  Run cp command

```
$ cp beanstalkcicd/lab-01/hello.js hello.js
```

2.  Check the sample code

```
$ cat hello.js

const express = require('express')
const app = express()
app.get('/', (req, res) => {
    res.send('Hello world from a Node.js app!')
})
app.listen(3000, () => {
    console.log('Server is up on 3000')
})
```

#### 1.3 Test sample Node REST API

1.  Run this command to host the REST API

```
$ node hello.js
```

2.  Open a new terminal

(./imgs/01/01.png)

3.  Run the curl command to test API

```
$ curl 'localhost:3000'

Hello world from a Node.js app!
```

We're done, continue to [Lab 2 : Create a sample Node API](./doc-module-02.md)
