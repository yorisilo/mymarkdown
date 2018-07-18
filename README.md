# mymarkdown

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).

/dist/index.html にはこんな感じのファイルがある
``` html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>mymarkdown</title>
  </head>
  <body>
    <div id="app"></div>
    <script src="https://www.gstatic.com/firebasejs/5.2.0/firebase.js"></script>
    <script>
      // Initialize Firebase
      var config = {
        apiKey: "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
        authDomain: "yorisilo-mymarkdown.firebaseapp.com",
        databaseURL: "https://yorisilo-mymarkdown.firebaseio.com",
        projectId: "yorisilo-mymarkdown",
        storageBucket: "",
        messagingSenderId: "111111111111"
      };
      firebase.initializeApp(config);
    </script>
    <script src="./build.js"></script>
  </body>
</html>
```

``` shell
> firease login
> firebas init # hosting mymarkdown dist
> npm run build
> firebase deploy
```
