<markdown>
# Dropdown

It is possible to pass a custom template when you want to customize the item link to be, for example a `dropdown` or a `router-link`.
</markdown>

<template>
  <n-breadcrumb>
    <n-breadcrumb-item>
      <n-dropdown :options="options1">
        I'm ok
      </n-dropdown>
    </n-breadcrumb-item>
    <n-breadcrumb-item>
      <n-dropdown :options="options2">
        I'm ok
      </n-dropdown>
    </n-breadcrumb-item>
  </n-breadcrumb>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup () {
    return {
      options1: [
        {
          label: 'David Tao',
          key: 1
        },
        {
          label: '黑色柳丁',
          key: 2
        }
      ],
      options2: [
        {
          label: '小镇姑娘',
          key: 1
        },
        {
          label: '普通朋友',
          key: 2
        }
      ]
    }
  }
})
</script>
