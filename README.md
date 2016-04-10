#Introduction

Defines a shareable jscs preset used by Kashoo for its javascript projects. This allows us to have a central file
defining a common javascript style.

#Usage

Projects that wish to use the Kashoo preset should first install a package that runs jscs, for example
[grunt-jscs](https://github.com/jscs-dev/grunt-jscs).

Once jscs is set up and running on the project, the next step is to install the kashoo preset: 

```
npm install jscs-preset-kashoo --save-dev
```

The kashoo preset can then be listed in the jscs config file as explained on the [jscs page](http://jscs.info/overview).
For example, a project can define its `.jscsrc` file to be

```
{
  "preset": "kashoo",
  "requireCurlyBraces": null // or false
}
```

This uses the kashoo preset and then adds any other desired rules on top of it.
