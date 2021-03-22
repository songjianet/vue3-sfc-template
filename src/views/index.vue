<template>
  <div class="layout-container">
    <div>
      <ant-u-i />
    </div>
    <div>
      <element-u-i />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import AntUI from '../components/AntUI.vue'
import ElementUI from '../components/ElementUI.vue'

export default defineComponent({
  name: 'index',
  components: { AntUI, ElementUI }
})
</script>

<style lang="scss" scoped>
.layout-container {
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: space-between;
  > div {
    width: calc(50% - 0.5px);
    height: inherit;
    &:first-child {
      border-right: 1px solid #e0e0e0;
    }
  }
}
</style>
