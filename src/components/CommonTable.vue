<template>
  <div>
    <el-table :data="tableData" tooltip-effect="light">
      <el-table-column label="User name" prop="name"></el-table-column>
      <el-table-column label="Desc." prop="desc"></el-table-column>
      <el-table-column label="Addresses" show-overflow-tooltip>
        <template #default="{ row }">
          {{ row.addresses.join('\n') }}
        </template>
      </el-table-column>
    </el-table>
  </div>
</template>

<script setup>
const tableData = [
  {
    name: 'zhangsan',
    desc: 'A nice man',
    addresses: [
      'Abet ex elit minim ullamco sint eu ut laboris eiusmod.',
      'Minim fugiat occaecat ipsum culpa laborum aute incididunt id.',
      'Proident qui minim enim et consectetur eiusmod.',
      'Est duis enim labore minim.',
      'Nulla quis eu qui ad voluptate.',
    ],
  },
];
</script>

<style>
.is-light {
  max-width: 330px !important;
}
.el-popper {
  white-space: pre-line !important;
}
</style>
