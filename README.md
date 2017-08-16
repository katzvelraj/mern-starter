**Note:** All the steps are tagged as 'step-1', 'step-2' and 'step-3'. Checkout at each step and give a try.

# Frontend - ReactJS

*Use `git checkout step-1`*

**Development Mode**

Runs a temporary server in local for easier development (say hotswapping changes)

Access Url: [http://localhost:3000](http://localhost:3000)

```
$ npm start
```
**Production Mode**

Transpiles (ES6 -> Old JS), Bundles (Single JS) and create a production ready static files.

Access Folder Name: `build/`

```
$ npm run build
```

# Backend - Node Server with Express Framework

*Use `git checkout step-2`*

Starts a actual server (same for development and production)

Access Url:  [http://localhost:5000](http://localhost:5000/api/user)

```
$ node server.js
```

# Using Pages and Api Calls via same domain

*Use `git checkout step-3`*

Production ready frontend pages are available in **'build'** folder

For api, Node server (in this example) is started in 5000 port [http://localhost:5000](http://localhost:5000)

Now we need to access the frontend pages ('build' folder) via node server. For this, we'll tell express to use 'build' folder using one line of code (See [here](https://github.com/rambabusaravanan/mern-starter/commit/942b6aea7125eba5894f783125cb09c3331e1913#diff-78c12f5adc1848d13b1c6f07055d996e))


### Important

Whenever you want to view both pages with api calls in action, always run `npm run build` followed by `node server.js`