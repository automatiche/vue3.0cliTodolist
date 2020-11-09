<template>
  <div class="form-group">
    <label for="exampleInputEmail1">添加待办</label>
    <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" v-model='inputValue'>
    <small id="emailHelp" class="form-text text-muted">回车即可加入</small>
  </div>
  <ul class="list-group">
    <li class="list-group-item">
       <div class="form-check">
        <input type="checkbox" class="form-check-input" id="exampleCheck1">
        <label class="form-check-label" for="exampleCheck1">Check me out</label>
      </div>
    </li>
  </ul>
</template>

<script lang='ts'>

import { defineComponent, reactive, ref } from 'vue'
export default defineComponent({
  setup () {
    const inputValue = ref('')
    return reactive({
      inputValue
    })
  }
})
</script>
<style scoped>

</style>
