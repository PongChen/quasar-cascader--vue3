<template>
  <q-page>
    <div class="row">
      <div class="col-md-2 col-sm-12 col-xs-12">
        <cascader
          label="单位"
          :options="data"
          dense
          optlabel="name"
          optvalue="id"
          @change="handleDeptIdChange"
          width="250"
        >
        </cascader>
      </div>
    </div>
  </q-page>
</template>

<script>
import cascader from "quasar-cascader-vue3";
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
