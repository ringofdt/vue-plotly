# Forked from [@rleys/vue-plotly](https://www.npmjs.com/package/@rleys/vue-plotly)

## Using plotly.js-cartesian-dist-min

Ref: <https://www.npmjs.com/package/plotly.js-cartesian-dist-min>

Ready-to-use minified plotly.js cartesian distributed bundle.

Contains trace modules scatter, bar, box, heatmap, histogram, histogram2d, histogram2dcontour, image, pie, contour, scatterternary and violin.

For more info on plotly.js, go to <https://github.com/plotly/plotly.js>

# vue-plotly

[![Npm version](https://img.shields.io/npm/v/@rleys/vue-plotly.svg)](https://www.npmjs.com/package/@rleys/vue-plotly) [![MIT License](https://img.shields.io/github/license/David-Desmaisons/vue-plotly.svg)](https://github.com/David-Desmaisons/vue-plotly/blob/master/LICENSE)

## Thin vue wrapper for [plotly.js](https://plot.ly/javascript/)

<span>It provides:</span>

- all methods and events of plotly.js-cartesian-dist-min
- data reactivity
- Redraw on resizing

![example](./example/assets/demo.gif)

## Live example

<https://david-desmaisons.github.io/vue-plotly/>

## Usage

```html
<Plotly :data="data" :layout="layout" :display-mode-bar="false"></Plotly>
```

```javascript
import { Plotly } from 'vue-plotly-cartesian'

export default {
  components: {
    Plotly
  },
  data:{
    data:[{
      x: [1,2,3,4],
      y: [10,15,13,17],
      type:"scatter"
    }],
    layout:{
      title: "My graph"
    }
  }
}
```

## API

### Props

- `data` **_Array_** (_optional_)

  [Data](https://plot.ly/javascript/reference/) to be displayed

- `layout` **_Object_** (_optional_)

  Graphic [layout](https://plot.ly/javascript/reference/#layout)

- `id` **_String_** (_optional_)

  Id of the root HTML element of the component.

- Others:

  Plotly component implements the [transparent wrapper pattern](https://zendev.com/2018/05/31/transparent-wrapper-components-in-vue.html):<br>
  All other props will be passed as plotly graphic [option](https://plot.ly/javascript/configuration-options/).

## Installation

```
npm install vue-plotly-cartesian
```

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Run your tests

```
npm run test
```

### Lints and fixes files

```
npm run lint
```

### Run your unit tests

```
npm run test:unit
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
