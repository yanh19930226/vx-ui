<template>
  <layout>
    <x-nav slot="header" back="/" title="Picker"></x-nav>
    <x-body slot="body">
      <message>注意：此示例要在移动设备体验哦~</message>
      <group :title="'value：'+value">
        <picker placeholder="请选择" v-model="value" :options="options"></picker>
      </group>
    </x-body>
  </layout>
</template>

<script>
import { children } from 'utils/mixins/page'
export default {
  mixins: [children],
  data () {
    return {
      options: [{
        value: '010101',
        label: '南山区'
      },
      {
        value: '010102',
        label: '福田区'
      },
      {
        value: '010103',
        label: '罗湖区'
      },
      {
        value: '010104',
        label: '宝安区'
      },
      {
        value: '010105',
        label: '龙华区'
      },
      {
        value: '010106',
        label: '龙岗区'
      },
      {
        value: '010107',
        label: '盐田区'
      },
      {
        value: '010108',
        label: '坪山区'
      },
      {
        value: '010109',
        label: '光明区'
      }],
      value: '010101'
    }
  }
}
</script>
