<template>
  <layout>
    <x-nav slot="header" back="/" title="Message"></x-nav>
    <x-body slot="body">
      <message>注意：此示例要在移动设备体验哦~</message>
      <br/>
      <message type="danger">注意：此示例要在移动设备体验哦~</message>
      <br>
      <message type="success">注意：此示例要在移动设备体验哦~</message>
    </x-body>
  </layout>
</template>
<script>
import { children } from 'utils/mixins/page'
export default {
  mixins: [children]
}
</script>
