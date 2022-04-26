# Weather Command
![Stable Version](https://img.shields.io/npm/v/weather.js)

<b>Weather Command coded with Discord.js (Version 13)</b>


## 📂 | Setup
`1.)` <p>Install the Package</p>
```console
npm i weather-js
```
`2.)` <p>Require the Module in your code</p>
```js
const weather = require('weather-js');
```
`3.)` <p>Getting the informations</p>
```js
weather.find({search:'Alabama', degreeType: "C"}, function(error, result){ // degreeType can also be "F" for Fahrenheit.
const current = result[0].current
const location = result[0].location
        
console.log(current.observationpoint) //Shows the name of the City
console.log(current.observationpoint) //Gives a short Description about the weather, example: "Light Rain".
console.log(current.temperature) //Gives current temperature.
console.log(current.winddisplay) //Gives current wind speed.
console.log(current.humidity) //Gives current humidity.
console.log(location.timezone) //Shows the Timezone of the current place.
})
```
## 👨🏼‍💻 | Example
<p> Here I am using <code>Slash Commands</code> and displaying the Gif in an <code>Embed</code>:</p>

[Example](https://github.com/yungbeatz/Weather-Command/blob/main/example.js)

