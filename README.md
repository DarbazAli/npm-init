## How to Use package.json, the Core of Any Node.js Project or npm Package
One of the most common pieces of information in this file is the author field. It specifies who created the project, and can consist of a string or an object with contact or other details. An object is recommended for bigger projects, but a simple string like the following example will do for this project.

`"author": "Jane Doe",`

## Add a Description to Your package.json
The next part of a good package.json file is `description` filed, where a short, but informative description about the project belongs.

`description` is a great way to summurize what is the project all about.
`"description": "A good project that solves a big problem"`

## Add keywords to the package.json
The keywords field is whre you can describe the project using related keyword.
```
"keywords": ["discriptive", "related", "words"]
```

## Add license to the package.json
The `license` field is whre you inform users of what they are allowed to do with your project.
```
"license": "MIT"
```

## Add Version to the package.json
A `version` is one of the required fields of you package.json file. This field describes the current version of your project.
```
"version": "1.2.0"
```

## Expand Your Project with External Packages from npm
One of the biggest reasons to use a package manager, is their powerful dependency management. Instead of manually having to make sure that you get all dependencies whenever you set up a project on a new computer, npm automatically installs everything for you. But how can npm know exactly what your project needs? Meet the `dependencies` section of your package.json file.

In this section, packages your project requires are stored using the following format:
```
"dependencies": {
  "package-name": "version",
  "express": "4.14.0"
}
```