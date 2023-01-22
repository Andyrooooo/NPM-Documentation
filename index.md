### What is NPM? What does it do? Why is it an important tool?
#### npm is a package manager consisting of JavaScript software and meta information, and is also the default package manager for Node.js. 
#### Essentially when you're using your terminal to download a package from node.js, which by the way is one of the largest ecosystems of libraries, npm will make a request to the registry to find that package for you, once it it found it will download the requested information and meta data associated with it. So, in short, any package request made will be managed by npm.
#### npm is an important tool because of automated dependency and package management. This greatly helps with collaboration and even just for your future self, so anytime you need to get started with the project or another person needs to start on the project they can just use npm to install all the dependencies for it. Another great positive for npm is you can specify what versions your project uses to prevent updates breaking the project.

### What problems does NPM Solve?
#### It makes the whole process of getting everything set up so much easier. Instead of having to find the library you want from some website, download it, and place it into your project, everything can be done straight from the npm. It overall made the process of creating projects much quicker and easier.

### Describe the 3 main parts of NPM.
####The three distinct components of npm are the website, the CLI (Command Line Interface), and the registry. The npm website allows you to discover packages, set up profiles, and manage any other aspects regarding npm. The CLI runs from a terminal and is where most of us will use npm to download and manage our packages. The last main component, the registry, is a large public database that contains all the JavaScript software and meta data. 

### What is the package.json file?
#### The package.json file is a json file that resides at the root of your node project. It contains metadata that is relevant to the project and is used to provide the information to npm that allows identifying your projects depencies, scripts, and version your using. Within that file you will see properties there or write properties like these: 
* **Name** - The name property in a package.json file is one of the fundamental components of the package.json structure. At its core, the name is a string that is the name of the module that the package.json is describing. The property only allows a maximum length of 214 URL friendly characters; no uppercase letters, no leading periods, and no underscores except for scoped packages. 

* **Version**- current version property tells you the current version of the module that the package.json file is describing.

* **Description** - brief description of the app/package

* **Dependencies** - The dependencies property module is defined by the other modules that the module uses. Each entry in the dependencies property includes the name and version of other packages required to run this package.

* **Main** - entry point for the application

* **browserlist** - this provides information about the browser compatibility of the app

* **Private** - if set to true prevents the app/package to be accidentally published on npm

* **Scripts** - a set of node scripts we can run

* **Keywords** - array of keywords that associate with what the package does

* **Author** - package author name

* **License** - license of the package

* **eslintConfig** - this property takes care of code linting, it will look for and read automatically, or you can specify a configuration file 

* **devDependencies** - The devDependencies property is almost identical to the dependencies property in terms of structure. The main difference: while the dependencies property is used to define the dependencies that a module needs to run in production, devDependencies property is commonly used to define the dependencies the module needs to run in development.

### What is the scripts section of the package.json file? How do you use it? What are the default commands, and how do you use your own?
#### The scripts property contains the aliases that we can use to access 

### What are dependencies? What does this section define? What are dev dependencies? Why is it important to define dev dependencies vs dependencies?

### How do you install dependencies? Where do dependencies get installed?

### When running scripts with NPM, where does NPM look (path) for the dependencies of those scripts?

### Name 3 NPM commands, and why they are important.
