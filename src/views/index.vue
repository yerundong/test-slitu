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
} from "slitu";

export default {
  name: "index",
  components: {},
  mounted() {
    // console.log(displaceByType(NaN, "aaaa", ["Number", "NaN"]));
    // console.log(displaceNil(undefined, 555));
    const value = jsonGetValue(
      [
        {
          value: 123,
          label: "aaa",
        },
        {
          value: 456,
          label: "bbb",
        },
      ],
      "label",
      "aaa"
    );
    console.log(value);
  },
};
</script>
