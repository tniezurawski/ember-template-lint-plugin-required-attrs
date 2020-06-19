# ember-template-lint-plugin-required-attrs

A plugin for [ember-template-lint](https://github.com/ember-template-lint/ember-template-lint) to lint your handlebars templates. It checks if required attributes are set on given tags.

That's very handy when you want for example all your `<input>`s having `name` or `id` tag so automated tests will be able to target them easily.

## Install

```sh
yarn add -D ember-template-lint-plugin-required-attrs
```

or 

```sh
npm install ember-template-lint-plugin-required-attrs --save-dev
```

As peerDependency, `ember-template-lint` has to be installed in your project.

## Recommended configuration

A recommended configuration is available. To use it, merge the following object
to your `.template-lintrc.js` file:

```
module.exports = {
  plugins: ["ember-template-lint-plugin-required-attrs"],

  extends: ["recommended", "ember-template-lint-plugin-required-attrs:recommended"],
  },
};
```
