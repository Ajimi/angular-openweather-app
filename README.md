# angular-openweather-app — a weather forecast app written in AngularJS

<img src="app/img/app_screenshot2_v_0-1-0.png" alt="OpenWeather App"/>

"OpenWeather App" is a small AngularJS project that makes use of the [OpenWeatherMap](http://openweathermap.org/)
API for displaying weather data and forecasts based on a given location (city).

_This project basically serves as an example app I refer to within an article/post about AngularJS
I'm going to publish for a German web technology magazine and in my blog._

angular-openweather-app is build upon:

* [AngularJS v1.2.0-rc.2](https://github.com/angular/angular.js) / [angular-seed](https://github.com/angular/angular-seed)
* [iso-3166-country-codes-angular](https://github.com/BluePyth/iso-3166-country-codes-angular)
* [Bootstrap v3.0.0](https://github.com/twbs/bootstrap)

Points of interests:

* Building an app with AngularJS
* Building an app based on a OpenWeatherMap
* Bootstrapping an AngularJS app: Basic modules and view definition, ng-app, ng-view
* Defining a controller for handling the weather data in $scope
* Defining a service for fetching weather data from openweathermap.com via JSONP
* Defining a custom directive for instantly embedding sort of "weather data day panel"
* Setting up unit and e2e-tests with karma/jasmine


## Installation

### Clone repository and install dependencies

via git and npm:

```
$ git clone git@github.com:atufkas/angular-openweather-app.git [my-app-name]
$ cd [my-app-name]
$ npm install
```

### Run application via server

(see also [angular-seed docs](https://github.com/angular/angular-seed))

You can pick one of these options:

* serve this repository with a webserver of-your-choice
* install node.js and run `scripts/web-server.js`

Then navigate your browser to `http://localhost:<port>/app/index.html` to see the app running in
your browser.


## Heads up! Related project "angular-openweather"

Setting up a service and directive for handling OpenWeatherMap data inspired me to extract those parts
and put it into a separate angular module-project called simply `angular-openweather` (coming soon).
It will probably be included as a dependency by this project later on. The original version of this app
I especially refer to in my post/article will always be available under the git tag tags/article-state.


## Contribute!

Ideas, suggestions and pull requests are welcome. Someone willing to suggest a fancy (responsive) design
for desktop and mobile use?


### Todo

* Make use (and parse) more provided weather data (+ add filters, formatting)
* Internationalization / Localization
* Provide "use current location" and fetch data via lat/lon
* Build a view with n-day-forecast in typical weather app style
* Improve UI/UX by integrating a fancy design, transitions, effects


## License

[The MIT License](http://opensource.org/licenses/MIT)

All data provided by the great service and API of [OpenWeatherMap](http://openweathermap.org/).

Copyright (c) 2013 Matthias Lienau &lt;matthias@mlienau.de&gt;