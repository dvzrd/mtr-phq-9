# Patient Health Questionnaire (PHQ-9)

Mobile-first PHQ-9 prototype built with React and Meteor.

> I decided to build this project in Meteor and React for a couple of reasons. I chose Meteor because it's a very fast way to prototype apps. I felt more comfortable in this environment because I've been working with it for a while now. Using react with Meteor is a good way to create your app's client while dealing with incoming data. The components are about 90% recyclable if they need to be plugged into another backend.

[VIEW THE DEMO](http://phq9.meteor.com)

* [Roadmap](#roadmap)
* [How to use](#how-to-use)
  * [Requirements](#requirements)
  * [Run Locally](#run-locally)
* [Structure](#structure)
  * [Packages used](#packages-used)
  * [Folder structure](#folder-structure)
* [License](#license)

## Roadmap

* Setup build environments and write tests
* Security (permissions, accounts, index by userId)
* Quotes Component tied to Collection
* Mobile native (cardovo, phonegap)
* Refactor code (see todos)

## How to use

### Requirements

Make sure [Meteor is installed and up to date](https://www.meteor.com/install) or run:

```
curl https://install.meteor.com/ | sh
```

### Run Locally

```
git clone git@github.com:amazingBastard/mtr-phq-9.git
cd mtr-phq-9
```

Run the following to get the bash file to work:

```
chmod +x ./run.sh
```

Now you can start the app with the following command:

```
./run.sh
```

The app should now be running on:

```
http://localhost:3000
```

## Structure

### Folder structure

```
app/                # Application folder
  client/             # Client folder
    components/          # Contains react components
      common/             # Common components (i.e. header, footer)
      doctors/            # Doctors modules / components
      elements/           # HTML elements components (i.e. forms, lists, buttons)
      layouts/            # Router layouts
      questions/          # Questions form modules / components
      quotes/             # Quotes modules / components
      reports/            # Reports modules / components
      views/              # All the views (routes)
    stylesheets         # LESS files (with autoprefixer)
      components/         # Components styles
        common/             # Common components styles
        doctors/            # Doctors module styles
        layouts/            # All layouts styles
        questions/          # Questions form module styles
        scores/             # Scores module styles
        views/              # All views (routes) styles
      elements.less       # html elements and modules styles
      helpers.less        # style helpers for global use
      typography.less     # global typigraphy styles
      variables.less      # All LESS variables
  collections/        # All Collections
  lib/                # Lib files that get executed first
  public/             # Public files
    images/             # Public image files
  router/             # All routes
  server/             # Server folder
    fixtures/           # Meteor.Collection fixtures defined
    methods/            # Server methods
    publications/       # Collection publications
    startup/            # On server startup
environments/       # Environments folder
  local/              # local environment
  production/         # production environment

```

### Packages Used

* Meteor Core
  * [meteor-base](http://github.com/meteor/meteor/tree/devel/packages/meteor-base)
  * [blaze-html-templates](https://github.com/meteor/meteor/tree/devel/packages/blaze-html-templates)
  * [react](http://github.com/meteor/meteor/tree/devel/packages/react)
  * [ecmascript](https://github.com/meteor/meteor/tree/devel/packages/ecmascript)
  * [es5-shim](https://github.com/meteor/meteor/tree/devel/packages/es5-shim)
  * [jquery](https://github.com/meteor/meteor/tree/devel/packages/jquery)
  * [mobile-experience](https://github.com/meteor/meteor/tree/devel/packages/mobile-experience)
  * [mongo](https://github.com/meteor/meteor/tree/devel/packages/mongo)
  * [session](https://github.com/meteor/meteor/tree/devel/packages/session)
  * [standard-minifiers](https://github.com/meteor/meteor/tree/devel/packages/standard-minifiers)
  * [tracker](https://github.com/meteor/meteor/tree/devel/packages/tracker)
  * [check](https://github.com/meteor/meteor/tree/devel/packages/check)
  * [fastclick](http://github.com/meteor/meteor/tree/devel/packages/fastclick)
* Routing
  * [kadira:flow-router](https://github.com/kadirahq/flow-router)
  * [kadira:react-layout](https://github.com/kadirahq/meteor-react-layout)
  * [meteorhacks:fast-render](https://github.com/meteorhacks/fast-render)
* SEO
  * [spiderable](http://github.com/meteor/meteor/tree/devel/packages/spiderable)
  * [tomwasd:flow-router-seo](https://github.com/tomwasd/flow-router-seo)
* UI and UX
  * [natestrauser:animate-css](https://github.com/nate-strauser/meteor-animate-css)
* Development
  * [flemay:less-autoprefixer](https://github.com/flemay/less-autoprefixer)
  * [msavin:mongol](https://github.com/msavin/Mongol)

## License

This project has an MIT License, see the LICENSE.txt for more information.
