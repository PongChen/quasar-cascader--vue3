<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    />
    <cascader
      label="单位"
      :options="data"
      dense
      optlabel="name"
      optvalue="id"
      @change="handleDeptIdChange"
    >
    </cascader>
  </q-page>
</template>

<script>
import cascader from "quasar-cascader-vue3/src";
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageIndex",
  data() {
    return {
      data: [
        {
          id: 8,
          name: "上海铁路局",
          parentId: 1,
          deptType: 2,
          children: [
            {
              id: 48,
              name: "合肥机务段",
              parentId: 8,
              deptType: 3,
              children: [
                {
                  id: 148,
                  name: "合肥机务段111",
                  parentId: 8,
                  deptType: 3
                },
                {
                  id: 111,
                  name: "南京东机务段111",
                  parentId: 8,
                  deptType: 3
                }
              ]
            },
            {
              id: 49,
              name: "南京东机务段",
              parentId: 8,
              deptType: 3
            },
            {
              id: 50,
              name: "上海机务段",
              parentId: 8,
              deptType: 3
            },
            {
              id: 51,
              name: "杭州机务段",
              parentId: 8,
              deptType: 3
            },
            {
              id: 52,
              name: "徐州机务段",
              parentId: 8,
              deptType: 3
            },
            {
              id: 126,
              name: "柳州机务段",
              parentId: 8,
              deptType: 3
            }
          ]
        }
      ]
    };
  },
  components: {
    cascader
  }
});
</script>
