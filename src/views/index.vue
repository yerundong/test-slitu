<template>
  <div>
    <strong>utils测试</strong>
  </div>
</template>

<script>
import {
  displaceByType,
  displaceNil,
  arrayToMap,
  mapToArray,
  mapToObject,
  jsonGetValue,
  Timer,
} from "slitu";

export default {
  name: "index",
  components: {},
  mounted() {
    // console.log(displaceByType(NaN, "aaaa", ["Number", "NaN"]));
    // console.log(displaceNil(undefined, 555));
    const timer = new Timer();
    let a = 0;
    for (let index = 0; index < 1000000; index++) {
      a += index;
    }
    console.log(a);
    timer.end();
    console.log(timer.getDiff());
  },
};
</script>
