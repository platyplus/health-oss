# Frontend

Most of the modern web-based applications are using a modern JavaScript framework. You can find countless [benchmarks](https://en.wikipedia.org/wiki/Comparison_of_JavaScript_frameworks) and presentations about them. This list picked the three main frameworks, as building health software requires a certain level of sustainability, meaning the underlying technologies must not become obsolete too quickly, and the skills and libraries must remain available in the long run.

## [Vue](https://vuejs.org/) <Badges user="vuejs" repo="vue" />

Vue is the most popular frontend framework based on its number of GitHub stars. It is lightweight and easy to learn, although it can be used as a basis for bigger applications. It works together with a simplistic and powerful [router](https://router.vuejs.org/) and [state manager](https://vuex.vuejs.org/).

Vue can be extended with components libraries such as [Vuetify](https://vuetifyjs.com/), or more robust frameworks that allows the delivery of cross-platform applications (desktop, Android, IOS, Windows, OSX) such as [Quasar](https://quasar.dev/). Quasar recently integrated [Capacitor](https://capacitor.ionicframework.com/), Ionic's hybrid application builder, to supersede Cordova. Both Vuetify and Quasar follow Google's [Material Design](https://material.io/) specifications.

## [React](https://reactjs.org/) <Badges user="facebook" repo="react" />

React has been created and is still backed by Facebook. React has the biggest open-source community, and countless libraries are available open-source. While React offers the biggest flexibility, its learning curve may be a bit steeper than Vue. The most common state manager in use in the React ecosystem is [Redux](http://redux.js.org), but [MobX](http://mobx.js.org) is catching up fast as some developer find it easier to use.

[React Native](https://facebook.github.io/react-native/) is very similar to React, and is design for developing mobile applications. Although its syntax is similar, and some libraries are shared, React and React Native are not fully interoperable, meaning the developer will still have to develop two separate applications working on a browser or a mobile device.

## [Angular](https://angular.io/) <Badges user="angular" repo="angular" />

Angular is historically the first modern frontend framework, created by Google. Its strict architecture and maturity keeps it attractive to the private sector (based on job market). Angular 2+ is not backward compatible with the initial AngularJS first version.

The most popular hybrid framework based on Angular is the [Ionic framework](https://ionicframework.com/). It allows to deliver hybrid applications running on the browser, Android, IOS, Windows and OSX. Ionic has been recently made available for React as well.

## Data visualisation

Data visualisation is a recurrent need in health software: patient dashboards, service monitoring, reporting...

### [ChartJS](http://www.chartjs.org/) <Badges user="chartjs" repo="Chart.js" />

Chart.js offers simple, clean and flexible charts. It is easy to integrate with any JavaScript framework, and offers nice features such as animated charts and mixed chart types. The number of chart types is deliberately small in order to keep a consistent and user interface.

### [D3](https://d3js.org) <Badges user="d3" repo="d3" />

D3 is a more complete library, and virtually allows any type of visualisation. However it has a slight steeper learning curve, and the types of visualisation sometimes differ on an user interface standpoint.

### [Leaflet](https://leafletjs.com/) <Badges user="Leaflet" repo="Leaflet" />

Leaflet is a mobile-friendly JavaScript library for interactive maps. It is designed with simplicity, performance and usability in mind. Although other libraries exist, Leaflet is a good balance between simplicity and exhaustiveness.

<!-- ## Progressive Web Apps

### Workbox -->
