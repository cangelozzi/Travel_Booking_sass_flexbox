
# Landing page for HOTEL TRAVEL BOOKING practicing SASS and FLEXBOX

## For Development environment
```javascript
npm run start
```

### On Desktop
![image](img/intro.png)

### On mobile
![image](img/mobile.png) 

### Packages

```
{
  "name": "trillo",
  "version": "1.0.0",
  "description": "Landing page for Trillo App - travel bookings using Flexbox",
  "main": "index.js",
  "scripts": {
    "watch:sass": "node-sass sass/main.scss css/style.css -w",
    "devserver": "live-server",
    "start": "npm-run-all --parallel devserver watch:sass",
    "compile:sass": "node-sass sass/main.scss css/style.comp.css",
    "prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.comp.css -o css/style.prefix.css",
    "compress:css": "node-sass css/style.prefix.css css/style.css --output-style compressed",
    "build:css": "npm-run-all compile:sass prefix:css compress:css"
  },
  "author": "Camillo",
  "license": "ISC",
  "devDependencies": {
    "autoprefixer": "^7.1.4",
    "concat": "^1.0.3",
    "node-sass": "^4.5.3",
    "npm-run-all": "^4.1.1",
    "postcss-cli": "^4.1.1"
  }
}
```