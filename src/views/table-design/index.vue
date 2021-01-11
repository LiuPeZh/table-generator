<template>
  <div class="table-design">
    <div class="table-design-left"></div>
    <div class="table-design-main"></div>
    <div class="table-design-right"></div>
  </div>
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'

export default defineComponent({
  setup() {
    const testNum = ref<number>(0)

    return {
      testNum
    }
  }
})
</script>

<style lang="scss">
.table-design {
  * {
    outline: 1px solid red;
  }
  display: flex;
  height: 100vh;
  .table-design-left,
  .table-design-main,
  .table-design-right {
    height: 100%;
  }
  .table-design-left {
    flex: 0 0 300px;
  }
  .table-design-main {
    flex: 1 0 auto;
  }
  .table-design-right {
    flex: 0 0 200px;
  }
}
</style>
