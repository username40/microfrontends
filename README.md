# microfrontends
Pet project to single-spa-microfrontends with vue.js independent apps

How to install:

1 - install GLOBALLY single-spa.js
2 - move into each folder and install dependencies
3 - move in this folders strictly in this order:
    - header (write in terminal yarn serve)
    - footer (write in terminal yarn serve)
    - map (write in terminal yarn serve)
    - chart (write in terminal yarn serve)
    - root-config (write in terminal yarn start)
all applications must working (use independent terminal for each)

if you have error in browser console (csp)
please go to root-cofig/src/index.ejs and comment meta-tag 'meta http-equiv="Content-Security-Policy...'