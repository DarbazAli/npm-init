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

## Manage npm Dependencies By Understanding Semantic Versioning
Knowing SemVer can be useful when you develop software that uses external dependencies (which you almost always do). One day, your understanding of these numbers will save you from accidentally introducing breaking changes to your project without understanding why things that worked yesterday suddenly don’t work today. This is how Semantic Versioning works according to the official website:
```
"package": "MAJOR.MINOR.PATCH"
```
The MAJOR version should increment when you make incompatible API changes. The MINOR version should increment when you add functionality in a backwards-compatible manner. The PATCH version should increment when you make backwards-compatible bug fixes. This means that PATCHes are bug fixes and MINORs add new features but neither of them break what worked before. Finally, MAJORs add changes that won’t work with earlier versions.

## Use the Tilde-Character to Always Use the Latest Patch Version of a Dependency

To allow an npm dependency to update to the latest PATCH version, you can prefix the dependency’s version with the tilde (~) character. Here's an example of how to allow updates to any 1.3.x version.
```
"package": "~1.3.8"
```

## Use the Caret-Character to Use the Latest Minor Version of a Dependency
Similar to how the tilde we learned about in the last challenge allows npm to install the latest PATCH for a dependency, the caret (^) allows npm to install future updates as well. The difference is that the caret will allow both MINOR updates and PATCHes.
```
"package": "^1.3.8"
```
This would allow updates to any 1.x.x version of the package.