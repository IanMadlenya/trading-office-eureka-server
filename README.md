# Trading Office - Eureka Server
[![Build Status](https://travis-ci.org/spolnik/trading-office-eureka-server.svg?branch=master)](https://travis-ci.org/spolnik/trading-office-eureka-server) [![codecov.io](https://codecov.io/github/spolnik/trading-office-eureka-server/coverage.svg?branch=master)](https://codecov.io/github/spolnik/trading-office-eureka-server?branch=master)

Trading Office is reference implementation of microservices architecture, based on Spring Boot. It's modeling part of post trade processing, mainly focused on receiving Fixml message and preparing confirmation for it.

- [Trading Office](#trading-office)
- [Eureka Server](#eureka-server)
- [Notes](#notes)

## Trading Office

- [Trading Office](https://github.com/spolnik/trading-office)

## Eureka Server
- spring boot application
- discovery service (Netflix Eureka)
- it enables registration of all rest services allowing on later discovery of them
- both services, allocation enricher and confirmation sender has indirect dependencies to existing services thanks to eureka discovery mechanism

Heroku: http://eureka-server.herokuapp.com/

![Component Diagram](https://raw.githubusercontent.com/spolnik/trading-office-eureka-server/master/design/eureka_server.png)

## Notes
- checking if [dependencies are up to date](https://www.versioneye.com/user/projects/56ad39427e03c7003ba41427)
