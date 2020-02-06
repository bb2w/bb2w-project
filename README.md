# Project

The Building Block To Web (BB2W) project aims to build a platform where it is possible to create and manage component-oriented applications, aiming to simplify the development of websites, web systems, SPA, Apps that are initially based on webview, and may be extended in the future Apps that use native build technology, also facilitating publication in production through an orchestrator or container, while also facilitating the creation and maintenance of complementary services such as databases, data analysis services, queues and any other necessary for these applications

# Orchestration / Cloud Servers

For those who do not have experience like Devops or even with the use of containers and virtual machines the project will have full integration with orchestration systems and cloud servers that have API to abstract all part of configuration and infrastructure scalability, by default the system will use Kubernetes + Docker, however it will be possible to create integration modules for other types of orchestrators and or cloud servers

Standard support list:
- Kubernetes + Docker - https://kubernetes.io
- Amazon Web Services (AWS) - https://aws.amazon.com/
- Digital Ocean - https://www.digitalocean.com/
- Google Cloud - https://cloud.google.com/
- Microsoft Azure - https://azure.microsoft.com/

# Containers

All applications created by the default platforms will be pre-configured for a Docker (https://www.docker.com/) environment, every development environment must run in a container provided by BB2W, being obviously possible to be manually configured in any operating system.

# Core

The application will be written purely in ES6 Javascript using NodeJS (https://nodejs.org) as the default application interpreter, obviously any module / plugin can be written in other languages such as Typescript (https://www.typescriptlang.org/), but it will not be incorporated in the application core, the node modules needed to run the core will be properly tested and must obey the good practices used by the market in order to maintain quality in the code, periodic updates with bug fixes and security flaws, thus maintaining high quality standards.

# Build

To maintain compatibility with all versions of NodeJS the core application will use the Babel module as standard (https://babeljs.io/), for frontend files generated from the development using the platform, by default Webpack (https) : //webpack.js.org/), other build methods can be configured by project.

# Test



# Plugins

Definition of plugins for BB2W and any and all complement to the application core that will be distributed through Node JS modules, preferably through NPM (https://www.npmjs.com/) and can be implemented through other methods following the good practices similar to the core, BB2W is committed to developing and keeping updated plugins for basic application operation.

Preferably, plugins should not require application reboot, only in specific cases that change core configurations or routes, the plugins may require in the package.json to reboot or rebuild the application, the installation of plugins occurred by means of a command in the terminal, via Application API or the graphical interface that will be made available at installation.

### The standard for developing plugins will be released and linked in this document as soon as possible

# IDE Core

The fully web interface will be developed using plugins compatible with Atom (https://atom.io/) and VSCode (https://code.visualstudio.com/), initially the base application aims to create the components, which could be used for the construction of the construction platform itself, thus being defined as IDE Core the set of basic functions of the IDE, listed below

**Navbar** - Access menu with support for the creation of items and sub-items by plugins and services, shortcuts, modeled in an easy way for customization by theme system

**Panels** - Side panels used to divide content submenus, by default located on the right, left and footer

**Vertical navbar** - It aims to facilitate the use of resources such as shortcuts, aimed at a more iconographic menu and can be used laterally

**Tooltips** - System of hints or subtitles that can be configured in all interface components and plugins

**contextmenu** - Menu accessible by clicking with the right mouse button, which can be assigned to any component and plugin

**Tabs** - Side or top flap system that can be used in any component or plugin, which has options for iconography, close button and drop down

**Treeview** - Treeview system that can be used to display files from a given directory, with options to rename file, drop down, multi levels

**Content panels** - Multi-screen content manager, where it is possible to order several screens with code or other type of functionality, still with the ability to organize several tabs as well as all IDEs available on the market