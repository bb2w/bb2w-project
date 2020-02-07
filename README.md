# Project

The Building Block To Web (BB2W) project aims to build a platform where it is possible to create and manage component-oriented applications, aiming to simplify the development of websites, web systems, SPAs, Apps that are initially based on webview, and may be extended in the future Apps that use native build technology, also facilitating publication in production through an orchestrator or container, while also facilitating the creation and maintenance of complementary services such as databases, data analysis services, queues and any other necessary for these applications

# Introduction

Why do a project like this? It is the first question of all and I will try to summarize, after more than 15 years of experience in the IT industry, working in companies as a programmer and doing business in the Startups market.

Obviously there are great programmers who know a certain language like nobody, these professionals have the ability to code complex entire systems, with quality, performance and security alone, yet deliver documented, standardized, tested records in time.

However, this is not the reality of 99% of the IT market in the world, and over the years it is increasingly difficult to find them, new developers tend to want to shorten the learning process, often giving up basic concepts that are very important to work with technology, and choose to use libraries and frameworks without understanding the process that occurs behind thousands of lines of code created by thousands of people, these professionals mostly deliver low quality software, without standardization, without documentation, without tests, that soon becomes a heavy legacy for companies, leaving only long hours of refactoring or the need to create the same project from scratch several times until reaching the minimum level accepted to stay in production.

Therefore, there is nothing more natural than having a platform that can optimize and facilitate development to meet the increasingly complex demands, without the need for large programmers involved, and also abstracting all the concepts and good practices that take years of study to become. catch up. This project allows people without programming knowledge to develop web systems, apps, websites, just focusing on business rules, moving highly customizable pre-made components, defining simple events and connecting complex services such as databases, cloud servers, memory managers in a way almost childlike.

Even for those who already have experience, the platform works as a facilitator to develop applications, and will allow customization via code, enhancing the range of features.

I guarantee that a good part of Startups and technology companies die for the time it takes to develop their prototypes, and for the time it takes to maintain their legacies, that's why a project like this is so important for the Web to be accessible to business and people.

# Orchestration / Cloud Servers

For those who do not have experience like Devops or even with the use of containers and virtual machines the project will have full integration with orchestration systems and cloud servers that have API to abstract all part of configuration and infrastructure scalability, by default the system will use Kubernetes + Docker, however it will be possible to create integration modules for other types of orchestrators and or cloud servers

Standard support list:
- Kubernetes + Docker - https://kubernetes.io
- Amazon Web Services (AWS) - https://aws.amazon.com/
- Digital Ocean - https://www.digitalocean.com/
- Google Cloud - https://cloud.google.com/
- Microsoft Azure - https://azure.microsoft.com/
- Heroku - https://www.heroku.com/

# Containers

All applications created by the default platforms will be pre-configured for a Docker (https://www.docker.com/) environment, every development environment must run in a container provided by BB2W, being obviously possible to be manually configured in any operating system.

# Core

The application will be written purely in ES6 Javascript using NodeJS (https://nodejs.org) as the default application interpreter, obviously any module / plugin can be written in other languages such as Typescript (https://www.typescriptlang.org/), but it will not be incorporated in the application core, the node modules needed to run the core will be properly tested and must obey the good practices used by the market in order to maintain quality in the code, periodic updates with bug fixes and security flaws, thus maintaining high quality standards.

# Build

To maintain compatibility with all versions of NodeJS the core application will use the Babel module as standard (https://babeljs.io/), for frontend files generated from the development using the platform, by default Webpack (https://webpack.js.org/), other build methods can be configured by project.

# Test

The application tests will be carried out using Chai(https://www.chaijs.com/), Mocha (https://mochajs.org/) and Supertest (https://github.com/visionmedia/supertest), so it will be possible to create a standardized structure of unit tests and HTTP tests, while maintaining the development standard ESLint (https://eslint.org/) will be used

# Plugins

Definition of plugins for BB2W and any and all complement to the application core that will be distributed through Node JS modules, preferably through NPM (https://www.npmjs.com/) and can be implemented through other methods following the good practices similar to the core, BB2W is committed to developing and keeping updated plugins for basic application operation.

Preferably, plugins should not require application reboot, only in specific cases that change core configurations or routes, the plugins may require in the **package.json** to reboot or rebuild the application, the installation of plugins occurred by means of a command in the terminal, API or the graphical interface that will be made available at installation.

### The standard for developing plugins will be released and linked in this document as soon as possible

# IDE

The fully web interface will be developed using plugins compatible with Atom (https://atom.io/) and VSCode (https://code.visualstudio.com/), initially the base application aims to create the components, which could be used for the construction of the construction platform itself, thus being defined as IDE Core the set of basic functions of the IDE, listed below

**Navbar** - Access menu with support for the creation of items and sub-items by plugins and services, shortcuts, modeled in an easy way for customization by theme system

**Panels** - Side panels used to divide content submenus, by default located on the right, left and footer

**Vertical navbar** - It aims to facilitate the use of resources such as shortcuts, aimed at a more iconographic menu and can be used laterally

**Tooltips** - System of hints or subtitles that can be configured in all interface components and plugins

**Contextmenu** - Menu accessible by clicking with the right mouse button, which can be assigned to any component and plugin

**Tabs** - Side or top flap system that can be used in any component or plugin, which has options for iconography, close button and drop down

**Treeview** - Treeview system that can be used to display files from a given directory, with options to rename file, drop down, multi levels

**Content panels** - Multi-screen content manager, where it is possible to order several screens with code or other type of functionality, still with the ability to organize several tabs as well as all IDEs available on the market

# Modules 

Below is the list of modules that will be used in the project for both structural features and layout, remembering that the IDE will be coded in Javascript and its frontend developed based on the Vuejs framework (https://vuejs.org/)

### IDE

**Layout** - Vuetify (https://vuetifyjs.com/)

**Contents panels** - GoldenLayout (https://golden-layout.com/)

**Terminal** - Node-pty (https://www.npmjs.com/package/node-pty), xterm (https://www.npmjs.com/package/xterm)

**Treeview** - Fancytree (https://github.com/mar10/fancytree)

**Shortcuts** - Mousetrap (https://craig.is/killing/mice)

**Scrollbar** - 

**Editor** - Monaco (https://github.com/Microsoft/monaco-editor)

### Services

As practically all web applications have at least one database integration, BB2W will be responsible for implementing and maintaining interface modules for services.

**Databases SQL** - MySQL (https://www.npmjs.com/package/mysql), PostgreSQL (https://www.npmjs.com/package/pg), MariaDB (https://www.npmjs.com/package/mariadb), SQL Server (https://www.npmjs.com/package/mssql), Oracle (https://www.npmjs.com/package/oracle)

**NoSQL** - MongoDB (https://www.npmjs.com/package/mongodb), Amazon DynamoDB (https://www.npmjs.com/package/aws-sdk), RethinkDB (https://www.npmjs.com/package/rethinkdb), Apache CouchDB (https://www.npmjs.com/package/nano), Apache Cassandra (https://www.npmjs.com/package/cassandra-driver)

**Memory** - Redis (https://www.npmjs.com/package/ioredis), Amazon ElastiCache (https://www.npmjs.com/package/aws-sdk), Memcached (https://www.npmjs.com/package/memcached)

**Search** - Elastic Search (https://www.npmjs.com/package/elasticsearch), Apache Solr (https://www.npmjs.com/package/solr-client)

**Graph Database** - Neo4j (https://www.npmjs.com/package/neo4j-driver)

**Metrics Database** - InfluxDB (https://www.npmjs.com/package/influx),

**Queuing** - RabbitMQ (https://www.npmjs.com/package/amqplib), Apache Kafka (https://www.npmjs.com/package/node-rdkafka)

**Storage** - Amazon S3 (https://www.npmjs.com/package/aws-sdk), Google Cloud Storage (https://www.npmjs.com/package/@google-cloud/storage), MinIO (https://www.npmjs.com/package/minio)

**Big Data** - Apache Spark (https://www.npmjs.com/package/eclairjs)

**OAuth** - Keycloak (https://www.npmjs.com/package/keycloak-connect), Passport (https://www.npmjs.com/package/passport)

**Email** - SendGrid (https://www.npmjs.com/package/@sendgrid/mail), Mailgun (https://www.npmjs.com/package/mailgun)

**SMS** - Till Mobile, Blower.io SMS

**Others** - GraphQL (https://www.npmjs.com/package/graphql)

### Integrations

**Git** - https://www.npmjs.com/package/nodegit
**New Relic** - https://www.npmjs.com/package/newrelic
**Google APIs** - https://www.npmjs.com/package/googleapis
**Firebase** - https://www.npmjs.com/package/firebase
