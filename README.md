# Trading Office [![Build Status](https://travis-ci.org/spolnik/trading-office.svg?branch=master)](https://travis-ci.org/spolnik/trading-office) [![codecov.io](https://codecov.io/github/spolnik/trading-office/coverage.svg?branch=master)](https://codecov.io/github/spolnik/trading-office?branch=master) [![Sonar Coverage](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office/coverage.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1) [![Sonar Tech Debt](https://img.shields.io/sonar/https/sonar-nprogramming.rhcloud.com/trading-office/tech_debt.svg)](https://sonar-nprogramming.rhcloud.com/dashboard/index/1) [![Coverity Scan Build Status](https://scan.coverity.com/projects/7604/badge.svg)](https://scan.coverity.com/projects/spolnik-trading-office)

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
