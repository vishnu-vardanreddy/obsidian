App.jsx
```
// import { useState } from 'react'

// import reactLogo from './assets/react.svg'

// import viteLogo from '/vite.svg'

import { Route, Routes } from 'react-router-dom'

import './App.css'

import {HomePage} from './Pages/HomePage/HomePage'

  

const App = () => {

  return (

  

     <>

     <div className="App">

      <Routes>

        <Route path="/" element = {<HomePage/>} />

      </Routes>

      <HomePage/>

     </div>

    </>

  );

};

  

export default App
```

``` main.jsx
import { StrictMode } from 'react';

import { createRoot } from 'react-dom/client';

import App from './App.jsx';

import './index.css';

import "bootstrap/dist/css/bootstrap.min.css";

import "bootstrap/dist/js/bootstrap.bundle";

import {Provider} from "react-redux";

import store from "./redux/store"

import { BrowserRouter } from 'react-router-dom';

  

createRoot(document.getElementById('root')).render(

  <Provider store = {store}>

    <BrowserRouter>

    <App/>

    </BrowserRouter>

    <App />

  </Provider>,

)
```