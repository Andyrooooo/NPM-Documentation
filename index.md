### What is NPM? What does it do? Why is it an important tool?
#### npm is a package manager consisting of JavaScript software and meta information, and is also the default package manager for Node.js. 
#### Essentially when you're using your terminal to download a package from node.js, which by the way is one of the largest ecosystems of libraries, npm will make a request to the registry to find that package for you, once it it found it will download the requested information and meta data associated with it. So, in short, any package request made will be managed by npm.
#### npm is an important tool because of automated dependency and package management. This greatly helps with collaboration and even just for your future self, so anytime you need to get started with the project or another person needs to start on the project they can just use npm to install all the dependencies for it. Another great positive for npm is you can specify what versions your project uses to prevent updates breaking the project.

### What problems does NPM Solve?
#### It makes the whole process of getting everything set up so much easier. Instead of having to find the library you want from some website, download it, and place it into your project, everything can be done straight from the npm. It overall made the process of creating projects much quicker and easier.

### Describe the 3 main parts of NPM.
#### The three distinct components of npm are the website, the CLI (Command Line Interface), and the registry. The npm website allows you to discover packages, set up profiles, and manage any other aspects regarding npm. The CLI runs from a terminal and is where most of us will use npm to download and manage our packages. The last main component, the registry, is a large public database that contains all the JavaScript software and meta data. 

### What is the package.json file?
#### The package.json file is a json file that resides at the root of your node project. It contains metadata that is relevant to the project and is used to provide the information to npm that allows identifying your projects depencies, scripts, and version your using. Within that file you will see properties there or write properties like these: 
* **Name** - The name property is a string that contains the name of the module. The property only allows a maximum length of 214 URL friendly characters; no uppercase letters, no leading periods, and no underscores except for scoped packages. 

* **Version**- version property tells you the current version of the module.

* **Description** - The description property is a string that contains a human-readable description of the module. It's a quick summary of what the module does. Typically when searching for packages using npm, the search tools will look through the descriptions for a match. 

* **Dependencies** - The dependencies property will include other modules that the module uses. Each entry in the dependencies property will include the name and version of other packages required to run this package.

* **Main** - the main property is an entry point for the application, when the module is called it will export the data from the file that is contained in the main property.

* **browserlist** - the browserlist property provides information about the browser compatibility of the app

* **Private** - the private property can be helpful when working on your project, if it is set to true, this prevents the app/package from accidentally being published on npm

* **Scripts** - the scripts property is a set of node scripts we can run, it typically starts with the name of the script followed by the value that is a user-defined command that will execute.

* **Keywords** - the keywords property is exactly what you would think it is, it is an array of keywords that identify the package, related modules, and software.

* **License** - The license property tells you what license is being used by the project, the most typical usage is to use an SPDX License identifier. An example you may know is MIT, ISC, and GPL-3.0. [spdx.org](https://spdx.org/licenses/) 🔗🔗

* **eslintConfig** - this property takes care of code linting, it will look for and read automatically, or you can specify a configuration file 

* **devDependencies** - The devDependencies property is almost identical to the dependencies property in terms of structure. Although, the dependencies property is used to define the dependencies that a module needs to run in production, devDependencies property is used to define the dependencies the module needs to run in development.

### What is the scripts section of the package.json file? How do you use it? What are the default commands, and how do you use your own?
#### As we said before the scripts property contains script commands that are then executed, these commands run at different times of the life cycle of your package. The life cycle event would be the name of your script or "key", and the value would be the script command that is run, this can typically range from a multitude of things for it to do. 
#### Now to use just this section of the package.json file, we can use some example code:
```# example code
"scripts": {
  "test": "ls",
  "build": "tsc"
}
```
#### Then in your command line you can execute this
`
npm test
`
#### Now, to execute commands that are not default you would typically execute "npm run ___"
`
npm run build
`
#### Within the scripts property there a quite a few of different default commands like start which starts a package, stop to stop a package, test to test a package, restart to restart a package and much, much more. [commands](https://docs.npmjs.com/cli/v9/commands?v=true) 🔗🔗
#### Now to create your own command you would simply give it the name and value within the object. Once you created the script you will use this in the command line as shown above with "npm run (command name)

### What are dependencies? What does this section define? What are dev dependencies? Why is it important to define dev dependencies vs dependencies?

### How do you install dependencies? Where do dependencies get installed?

### When running scripts with NPM, where does NPM look (path) for the dependencies of those scripts?

### Name 3 NPM commands, and why they are important.
