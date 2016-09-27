# Canvas gauges

Canvas gauges component is based on [canvas-gauges](https://canvas-gauges.com/) for Vue Bulma.

## Installation

```
$ npm install vue-canvas-gauges --save
```

## Examples

```vue
<template>
  <div>
    <radial-gauge options="{ value: 233 }"></radial-gauge>
    <linear-gauge :value="377"></linear-gauge>
  </div>
</template>

<script>
import { LinearGauge, RadialGauge }  from 'vue-canvas-gauges'

export default {
  components: {
    LinearGauge,
    RadialGauge
  }
}
</script>

```


## Badges

![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

---

> [fundon.me](https://fundon.me) &nbsp;&middot;&nbsp;
> GitHub [@fundon](https://github.com/fundon) &nbsp;&middot;&nbsp;
> Twitter [@_fundon](https://twitter.com/_fundon)
