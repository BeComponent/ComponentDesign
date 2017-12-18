# Component Design

##### Resources slides

https://github.com/russellgoldenberg/scrollama


##### Resources

- [x] [6 reasons component based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)
      - Ensure **consistency** within a portfolio of applications

      - Steps to switch to component based UI

        1. Identify candidates ( list components and rank them depending on level of re-use)
        2. Establish a component library framework
        3. Focus on isolation (components should be independents)

        ​


- [x] [Understanding Component-Based Architecture](https://medium.com/@dan.shapiro1210/understanding-component-based-architecture-3ff48ec0c238)


MVC vs CBA => MVC split responsabilities **horizontally** whereas CBA split them **vertically**

- [x] [Create atomic design systems with Pattern Lab.](http://patternlab.io/)


- [x] [UI Component Playbook](https://blog.hichroma.com/ui-component-playbook-fd3022d00590)



- [x] [Presentational and Container Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0)

      **Presentational**

      - How things look
      - Contain both presentational and containers components
      - No dependencies on the rest of the app
      - Don't specify data loading or mutation
      - Data and callbacks throught props
      - No own state

      **Container**

      - How things work
      - Contain both presentational and containers components
      - No markup (other than components)
      - No style
      - Provide Data and behavior
      - Call actions
      - Stateful

      => Provide better separation of concerns

      => Presentational can be put on a page listing them and designers can modify their style without touching logic code.

      To introduce containers, start by moving every components to presentational ones, when we realize that we have to pass to many data through props and some components are only hatch it means that we have to create containers.



- [ ] [Micro frontends](https://micro-frontends.org/)



- [x] https://dassur.ma/things/120fps/
  - [ ] https://developers.google.com/web/showcase/2016/service-worker-perf

  __Service Worker :__
  Background service that handles network requests. Ideal for dealing with offline situations and background syncs or push notifications. Cannot directly interact with the DOM. Communication must go through the Service Worker’s `postMessage` method.
  __Web Worker:__
  Mimics multithreading, allowing intensive scripts to be run in the background so they do not block other scripts from running. Ideal for keeping your UI responsive while also performing processor-intensive functions. Cannot directly interact with the DOM. Communication must go through the Web Worker’s `postMessage` method.
  __WebSocket:__
  Creates an open connection between a client and a server, allowing persistent two-way communication over a single connection. Ideal for any situation where you currently use long-polling such as chat apps, online games, or sports tickers. Can directly interact with the DOM. Communication is handled through the WebSocket’s `send` method.


- [x] [Component Driven Development](https://blog.hichroma.com/component-driven-development-ce1109d56c8e)
  __Benefits__
  - Focus development
  - Increase UI coverage
  - Target feedback (just like in a small MR/PR)
  - Build a component library
  - Parallelize development (see micro-frontend)
  - Test visually


- [x] [Higher Order Component](http://putaindecode.io/fr/articles/js/react/higher-order-component/)
- [ ] [React patterns](https://www.youtube.com/watch?v=BJdg56yrG84)
- [ ] [Atomic Design, Brad Frost, InVision](https://www.invisionapp.com/blog/design-systems-brad-frost/?utm_campaign=Weekly%20Digest&utm_source=hs_email&utm_medium=email&utm_content=58639578&_hsenc=p2ANqtz-_wcWXY18-ISf4e90cwWNJizvQQ5-y1wcTdEkcikPvk0ti8Uk9LMtWnbY0wbndDUJrdtAmIyRZ2cI1g6DJYuddzDAnJhSZjEg0Ns0ilghr7EKqPNSI&_hsmi=58639580) 
- [ ] https://twitter.com/Real_CSS_Tricks/status/942424145517842433

## 💡Idea

Create slides with components using [spectacle](https://github.com/FormidableLabs/spectacle) or [reveal.js](https://github.com/hakimel/reveal.js/)



## WHY

Because we believe that frontend development isn't just about scripting in one file to refresh data with AJAX and it is a big challenge to create robust and well designed application.

## HOW

We have to embrace advanced patterns to architecture our projects

## WHAT

To do so, we will present you patterns for introduce component design into your applications

## Conflict

Have to work on application to improve them and add features, but the point is that often it is not well isolated, there is to many dependencies between parts of application. You just have to remove a props of a component and your console is all red.

## Resolution

### Different patterns

#### Design guidelines

#### Dumb/smart (container/presentational)

#### Atomic Design

#### Micro frontend

