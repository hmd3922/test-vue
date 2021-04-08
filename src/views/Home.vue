<template>
  <div>
    <base-table :list="list">
      <thead>
        <tr>
          <th v-for="item in thDataList" :key="item">{{ item.name }}</th>
        </tr>
      </thead>
    </base-table>
  </div>
</template>
<script>
import baseTable from "@/components/HelloWorld";
export default {
  components: {
    baseTable,
  },
  data() {
    return {
      thDataList: [
        {
          name: "矿种名称",
        },
        {
          name: "单位",
        },
        {
          name: "资源储量",
        },
        {
          name: "增减(%)",
        },
      ],
      list: [
        [
          {
            row: 1,
            val: "1",
          },
          {
            val: "2",
          },
          {
            val: "1",
          },
          {
            val: "2",
          },
        ],
        [
          {
            val: "2",
          },
          {
            val: "1",
          },
          {
            val: "2",
          },
          {
            val: "2",
          },
        ],
        [
          {
            col: 1,
            val: "2",
          },
          {
            val: "1",
          },
          {
            val: "2",
          },
          {
            val: "2",
          },
        ],
      ],
    };
  },
  computed: {},
  methods: {},
  mounted() {},
};
</script>
<style lang="less" scoped></style>
