<template>
  <div>
    <keep-alive>
      <router-view v-if="$route.meta.keepAlive"></router-view>
    </keep-alive>
    <router-view v-if="!$route.meta.keepAlive"></router-view>
  </div>
</template>

<script>
  export default {
    'name': 'App',
    data () {
      return {};
    },
    created () {
    },
  };
</script>

<style>
  @import "./assets/css/common/public.css";
</style>
