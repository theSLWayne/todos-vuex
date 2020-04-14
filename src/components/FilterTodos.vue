<template>
    <div>
        Todo Filter:
        <Select @change="filterTodos($event)">
          <Option value="200">200</Option>
          <Option value="100">100</Option>
          <Option value="50">50</Option>
          <Option value="20">20</Option>
          <Option value="10">10</Option>
        </Select>
    </div>
</template>

<script>
import { mapActions } from 'vuex'
export default {
    name: "FilterTodos",
    methods: {
        ...mapActions(['filterTodos'])
    },
}
</script>

<style scoped>
Select{
    margin-top: 20px;
    padding: 6px;
    border: #41b883 soild 1px;

}
</style>