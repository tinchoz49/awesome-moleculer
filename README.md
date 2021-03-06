<div align="center">
	<img width="500" height="350" src="media/awesome_moleculer.svg" alt="logo of awesome-moleculer repository">
	<br>
	<p>
		<a href="https://moleculer.services/support.html">Moleculer is supported by the community</a>
	</p>
	<br>
</div>

# Awesome Moleculer [![Mentioned in Awesome Node.js](https://awesome.re/mentioned-badge.svg)](https://github.com/sindresorhus/awesome-nodejs)

>A list of awesome things related to Moleculer microservices framework

- [Resources](#resources)
	- [Official Resources](#official-resources)
	- [Cheatsheets](#cheatsheets)
	- [Articles and Blog Posts](#articles-and-blog-posts)
- [Examples](#examples)
- [Services](#services)
	- [Gateways](#gateways)
	- [Databases & stores](#databases-&-stores)
	- [Metrics & Tracing](#metrics-&-tracing)
	- [General](#general)
	- [Others](#others)
- [Middlewares](#middlewares)
- [Mixins & Hooks](#mixins--hooks)
	- [Tasks, Queues & Jobs](#tasks-queues-&-jobs)
- [Tools](#tools)
- [Projects Using Moleculer](#projects-using-moleculer)

--------

## Resources

### Official Resources
- [Website](https://moleculer.services/)
- [Docs](https://moleculer.services/docs)
- [Blog](https://medium.com/moleculer)
- [Gitter](https://gitter.im/moleculerjs/moleculer)
- [Twitter](https://twitter.com/MoleculerJS)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/moleculer)


### Cheatsheets
- [Core Cheatsheets](https://github.com/moleculerjs/moleculer-cheatsheets/blob/master/moleculer.js) - Cheatsheet for Moleculer's core functionalities
- [Web Gateway Cheatsheets](https://github.com/moleculerjs/moleculer-cheatsheets/blob/master/moleculer-web.js) - Cheatsheet for official gateway
- [DB Cheatsheets](https://github.com/moleculerjs/moleculer-cheatsheets/blob/master/moleculer-db.js) - Cheatsheet for official DB adapaters
- [REPL Cheatsheets](https://github.com/moleculerjs/moleculer-cheatsheets/blob/master/moleculer-repl.sh) - Cheatsheet for official RELP tool
- [CLI Cheatsheets](https://github.com/moleculerjs/moleculer-cheatsheets/blob/master/moleculer-cli.sh) - Cheatsheet for Moleculer's command-line interface (CLI)

### Articles and Blog Posts

- [5 easy steps to create your REST microservice in NodeJS](https://medium.com/moleculer/5-easy-steps-to-create-your-rest-microservice-in-nodejs-94aede3249fc)
- [What are microservices and how to create one with Node and Moleculer.js](https://medium.com/@r.heygate.dev/microservices-with-moleculer-js-c7e68803ec09)
- [Moleculer — deployment thoughts](https://dankuida.com/moleculer-deployment-thoughts-8e0fc8c0fb07)
## Examples

- [Conduit](https://github.com/moleculerjs/moleculer-examples/tree/master/conduit) -  Moleculer + Moleculer Web + Moleculer-DB + MongoDB + JWT + Redis Cacher + Docker
- [Blog](https://github.com/moleculerjs/moleculer-examples/tree/master/blog) - Moleculer + ExpressJS + Pug + Moleculer-DB + Mongoose + NATS + Redis Cacher + Traefik
- [Kanban - A Kanban board application](https://github.com/icebob/kantab) - Moleculer + Moleculer Web + Full authentication + ACL/RBAC + VueJS + VueX + Vue-router + Much much more

## Services

### Gateways
- [moleculer-web](https://moleculer.services/docs/moleculer-web.html) ![Official Moleculer Module](media/moleculer-tiny.png) - HTTP gateway
- [moleculer-graphql](https://github.com/MerlinLabs/moleculer-graphql#readme) - GraphQL Schema stitching over a microservice network for co-located type definitions.
- [moleculer-sc](https://github.com/tiaod/moleculer-sc#readme) - API Gateway using SocketCluster
- [hapi-moleculer](https://github.com/felipegcampos/hapi-moleculer) - Hapi-based HTTP gateway
- [moleculer-io](https://github.com/tiaod/moleculer-io) - Socket.IO-based gateway

### Databases & Stores
- [moleculer-db](https://github.com/moleculerjs/moleculer-db/tree/master/packages/moleculer-db#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - A [NeDB](https://github.com/louischatriot/nedb)-based service to persist your data
- [moleculer-db-adapter-mongo](https://github.com/moleculerjs/moleculer-db/tree/master/packages/moleculer-db-adapter-mongo#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - A [MongoDB](https://mongodb.github.io/node-mongodb-native/)-based service to persist your data
- [moleculer-db-adapter-mongoose](https://github.com/moleculerjs/moleculer-db/tree/master/packages/moleculer-db-adapter-mongoose#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - A [Mongoose](https://mongoosejs.com/)-based service to persist your data
- [moleculer-db-adapter-sequelize](https://github.com/moleculerjs/moleculer-db/tree/master/packages/moleculer-db-adapter-sequelize#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - A [Sequelize](http://docs.sequelizejs.com/)-based service to persist your data

### Metrics & Tracing
- [moleculer-console-tracer](https://github.com/moleculerjs/moleculer-metrics/tree/master/packages/moleculer-console-tracer#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Console-based service
- [moleculer-jaeger](https://github.com/moleculerjs/moleculer-metrics/tree/master/packages/moleculer-jaeger#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - [Jaeger](https://www.jaegertracing.io/)-based metrics service
- [moleculer-prometheus](https://github.com/moleculerjs/moleculer-metrics/tree/master/packages/moleculer-jaeger#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - [Prometheus](https://prometheus.io/)-based metrics service
- [moleculer-zipkin](https://github.com/moleculerjs/moleculer-metrics/tree/master/packages/moleculer-zipkin#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - [Zipkin](https://zipkin.io/)-based metrics service
- [moleculer-elastic-apm](https://github.com/intech/moleculer-elastic-apm#moleculer-elastic-apm) ![Official Moleculer Module](media/moleculer-tiny.png) - [Elastic APM](https://www.elastic.co/solutions/apm)-based metrics service

### General
- [moleculer-fake](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-fake#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Fake data generator by [Fakerator](https://github.com/icebob/fakerator)
- [moleculer-mail](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-mail#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Email service based on [Nodemailer](https://nodemailer.com/about/)
- [moleculer-twilio](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-twilio#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - SMS service based on [Twilio  API](https://www.twilio.com/docs/usage/api)
- [moleculer-slack](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-slack#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Send Messages to [Slack API](https://api.slack.com/)
- [moleculer-flydrive](https://github.com/molobala/moleculer-flydrive#readme) -  Storage manager service with [Node Flydrive](https://github.com/Slynova-Org/node-flydrive)
- [moleculer-markdown](https://github.com/alsofronie/moleculer-markdown#readme) - Markdown to HTML Service

### Others
- [imicros-flow](https://github.com/al66/imicros-flow) - Service for loose coupled event handling
- [moleculer-vault](https://github.com/designtesbrot/moleculer-vault) - Service for [HashiCorp's Vault](https://www.vaultproject.io/)
- [moleculer-antivirus](https://github.com/designtesbrot/moleculer-antivirus) - Service for [ClamAV](https://www.clamav.net/) Antivirus Scanning

## Middlewares


## Mixins & Hooks
### Tasks, Queues & Jobs
- [moleculer-bee-queue](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-bee-queue#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Task queue mixin for [Bee-Queue](https://github.com/bee-queue/bee-queue)
- [moleculer-bull](https://github.com/moleculerjs/moleculer-addons/tree/master/packages/moleculer-bull#readme) ![Official Moleculer Module](media/moleculer-tiny.png) - Task queue mixin for [Bull](https://github.com/OptimalBits/bull)
- [moleculer-cron](https://github.com/davidroman0O/moleculer-cron#readme) - Cron mixin [Node-Cron](https://github.com/kelektiv/node-cron) 


## Tools
- [moleculer-repl](https://moleculer.services/docs/0.13/moleculer-repl.html) ![Official Moleculer Module](media/moleculer-tiny.png) - Interactive developer console
- [moleculer-cli](https://moleculer.services/docs/0.13/moleculer-cli.html) ![Official Moleculer Module](media/moleculer-tiny.png) - Command-Line Tool for development & testing
- [moleculer-decorators](https://moleculer.services/docs/0.13/services.html#Use-decorators) - ES7/TS decorators for Service declaration



## Projects Using Moleculer
- [Concierge Auctions](https://www.conciergeauctions.com/)
- [ingenious](http://www.ingsw.com/)
- [THB](https://www.thb.co.in/)
- [Zaoblako](https://zaoblako.ru/)
- [Altcoin mining pools](http://altcoinminingpools.com)
- [zebbra](https://zebbra.ch/)
- [Uiza](https://uiza.io)
- [Distopik](https://www.mixanalog.com)
- [AMRetail](http://amretail.ru)
- [DAZTA](https://dazta.com)
- [SmartTones Media](http://www.smarttonesmedia.com/)
- [Helpster](https://www.helpster.asia/id/business-en/)
- [Textalk](https://www.textalk.com/)
- [GetTechDone](https://www.gtechd.com/)
- [Jarvify](https://jarvify.com/)
- [Sonda](https://www.sonda.com/en/)

> IIf you don't see your company here, [tell us](https://github.com/moleculerjs/moleculer/issues/101).

# Contact
Copyright (c) 2016-2018 MoleculerJS

[![@moleculerjs](https://img.shields.io/badge/github-moleculerjs-green.svg)](https://github.com/moleculerjs) [![@MoleculerJS](https://img.shields.io/badge/twitter-MoleculerJS-blue.svg)](https://twitter.com/MoleculerJS)
