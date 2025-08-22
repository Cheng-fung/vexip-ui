<template>
  <Collapse v-model:expanded="expanded1" :alive="false">
    <CollapsePanel title="面板一">
      <Input></Input>
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
    <CollapsePanel title="面板二">
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded2" :alive="true">
    <CollapsePanel title="面板一">
      <Input></Input>
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
    <CollapsePanel title="面板二">
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded3" alive="after-loading">
    <CollapsePanel title="面板一">
      <Input></Input>
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
    <CollapsePanel title="面板二">
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
  </Collapse>
  <br />
  <br />
  <Collapse v-model:expanded="expanded4">
    <CollapsePanel title="面板一">
      <Input></Input>
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
    <CollapsePanel title="面板二" alive="always">
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
    </CollapsePanel>
    <CollapsePanel title="面板三" alive="after-loading">
      <p>一些内容一些内容一些内容</p>
      <p>一些内容一些内容一些内容</p>
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
