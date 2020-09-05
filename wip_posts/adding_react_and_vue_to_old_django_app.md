## React

https://medium.com/@dougmacknz/how-to-integrate-react-into-an-existing-multi-page-app-b727c2483ec4

https://reciosonny.com/how-to-integrate-reactjs-in-existing-asp-net-mvc-app/

```
npm install react react-dom --save

npm install webpack webpack-cli --save-dev
```

```
npm i @babel/core babel-loader @babel/preset-env @babel/preset-react --save-dev
```

```
    <div id="root"></div>
```

```
import React from 'react';
import ReactDOM from 'react-dom';

const App = () => <div>Hello world!</div>;

ReactDOM.render(<App />, document.getElementById('root'));

```

```
    <script src="{% static 'dist/index.js' %}"></script>
```

GEThttp://172.16.127.128/static/dist/test.js
[HTTP/1.1 404 Not Found 4ms]

due to djangos collect static system, forgot to run that so the file wasnt in static




## VUE

npm install @vue/cli --save-dev

npm install vue

npm install --save-dev eslint eslint-plugin-vue@next

npm install vue-loader vue-template-compiler webpack webpack-cli babel-loader @babel/core @babel/preset-env html-webpack-plugin -D

https://appdividend.com/2018/03/12/how-to-setup-vue-js-with-webpack-4-example/

https://www.freecodecamp.org/news/how-to-create-a-vue-js-app-using-single-file-components-without-the-cli-7e73e5b8244f/

https://stackoverflow.com/questions/33628558/vue-js-change-tags


# Both
npm install jest -D

in package.json

```json
"test": "jest"
```

