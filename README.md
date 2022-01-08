# Node Application Template

This is the template for you to use as the starting base of your node applications, it uses TypeScript and esLint for development, and Babel to compile the code and send it to production.

## Table of contents

<p>
  <dl>
    <dt><a href="#how-to-use">How to use?</a></dt>
    <dt><a href="#tips-for-using">Tips for using</a></dt>
    <dd><a href="#defining-paths-with-typescript">Defining paths with TypeScript</a></dd>
  </dl>
</p>

---

## How to use?

Clone this repository on your machine:

``` shell
$ git clone https://github.com/Suares01/App_Node_Template.git
```

Remove the `.git` folder.

``` shell
$ rm -rf .git
```

If you use PowerShell.

```PowerShell
$ rm -r -fo .git
```

You can now launch your own repository.

Now, install the dependencies.

``` shell
$ npm install
```

**And ready! You can start coding!**

[back](#node-application-template)

---

## Tips for using

### Defining paths with TypeScript

If you use the paths to TypeScript functionality. (`tsconfig.json` file)

```json
{
  "baseUrl": ".",
  "paths": {
    "@example/*": ["./src/example/*"]
  }
}
```

You also need to define these paths in the `.babelrc` file.

```json
{
  [
    "module-resolver",
    {
      "alias": {
        "@example": "./src/example"
      }
    }
  ]
}
```

[back](#node-application-template)
