# cron-editor-material-style

`cron-editor-material-style` is Material design CSS styles for [cron-editor](https://github.com/claudiuconstantin/cron-editor).

## Installation

This extension is published as a [npm package](https://www.npmjs.com/package/cron-editor-material-style).

```
npm install cron-editor-material-style --save
```

## Usage

Use class `cron-editor-material-control` in `CronOptions`:

```ts
cronOptions: CronOptions = {
  formInputClass: 'cron-editor-material-control',
  formSelectClass: 'cron-editor-material-control',
  ...
};
```

In your component styles use:

```scss
::ng-deep {
  @import "~cron-editor-material-style/scss/mixin";
  @include cron-editor-material-style($color);
}
```

where `$color` is the color of active tab or active input field. Default value: `#3f51b5`.

If you are not using Sass, then use a precompiled CSS:

```
~cron-editor-material-style/css/cron-editor-material-style.css
```

## Development

#### 1. Install dependencies

```
npm install
```

#### 2. Build CSS

```
npm run build
```

## License
Licensed under the MIT license.
