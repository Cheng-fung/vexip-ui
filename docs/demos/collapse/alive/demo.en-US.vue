<template>
  <Collapse v-model:expanded="expanded1" :alive="false">
    <CollapsePanel title="Panel 1">
      <Input></Input>
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
    <CollapsePanel title="Panel 2">
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded2" :alive="true">
    <CollapsePanel title="Panel 1">
      <Input></Input>
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
    <CollapsePanel title="Panel 2">
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded3" alive="after-loading">
    <CollapsePanel title="Panel 1">
      <Input></Input>
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
    <CollapsePanel title="Panel 2">
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded4">
    <CollapsePanel title="Panel 1">
      <Input></Input>
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
    <CollapsePanel title="Panel 2" alive="always">
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
    <CollapsePanel title="Panel 3" alive="after-loading">
      <p>Some content to fill</p>
      <p>Some content to fill</p>
    </CollapsePanel>
  </Collapse>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const expanded1 = ref()
const expanded2 = ref()
const expanded3 = ref()
const expanded4 = ref()
</script>

<style scoped>
.vxp-collapse {
  max-width: 500px;
}
</style>
