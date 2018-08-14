# Contributing to scrumoji

Hello!

Thanks for contributing on [scrumoji](https://github.com/oschrenk/scrumoji). Before implementing new features and changes, feel free to [submit an issue](https://github.com/oschrenk/scrumoji/issues/new). We're going to talk here :stuck_out_tongue_winking_eye:.

If you would like to add a new emoji to scrumoji, fill the provided `ISSUE_TEMPLATE` when creating an issue and take a look at the contributing section.

## How to submit a pull request?

1. Fork [this repository](https://github.com/oschrenk/scrumoji/fork).
2. Create a new branch with the feature name. (Eg: add-emoji-deploy, fix-website-header)
3. Make your changes.
4. Commit your changes. Don't forget to add a commit title with an emoji and a description.
5. Push your changes.
6. Submit your pull request.

## How to add a scrumoji

1. Open the **scrumojis.json** file located at `src/data/scrumojis.json`.
2. Add your emoji using the following code inside of the `scrumojis array []`:
3. Save the file and create a pull request.

```json
{
  "emoji": "",
  "code": ":code:",
  "description": "Enter the description for the scrumoji.",
  "name": "code (same as code but without ':' replace underscores for dashes _ => - )"
}
```

## How to start scrumoji and update

If you want to make changes to the site, follow the next steps:

1. Clone scrumoji

```bash
$ git clone https://github.com/oschrenk/scrumoji.git
$ cd scrumoji
```

2. Install the dependencies and start the development task.

```bash
$ npm i && gulp
```

3. Make sure the styles are using a link instead of being inlined.

_If you are updating the SCSS files and the styles doesn't get updated, go to the `index.pug` and `about.pug` paste the following code_

```jade
link(href="css/style.css", type="text/css", rel="stylesheet")
```

_Remove this one_

```jade
style
  include ../../dist/css/style.css
```

**After making your changes, inline the styles as before.**

The project is built with [Pug](http://pugjs.org) and [SCSS](http://sass-lang.com)
