<!--
 * @Descripttion: Spicy chicken
 * @Author: YuShu Xiao
 * @Date: 2023-02-06 11:57:03
 * @LastEditors: Huccct
 * @LastEditTime: 2023-02-08 11:22:23
-->
<template>
  <div class="tas-bread-item">
    <RouterLink v-if="to" :to="to"><slot /></RouterLink>
    <span v-else><slot /></span>
    <tass-icon name="chevronright"></tass-icon>
  </div>
</template>
<script setup lang="ts" name="TassBreadcrumbItem">
  import '../style/';
  defineProps({
    to: {
      type: [String, Object]
    }
  });
</script>
