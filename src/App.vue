<template>
  <main class="gpt">
    <div class="menu">
      <MenuList />
    </div>
    <div class="content">
      <RouterView />
    </div>
  </main>
</template>

<script setup>
import MenuList from './components/MenuList.vue';
  
</script>

<style lang="less">
.gpt{
  display: flex;
  flex-direction: row;
  .menu{
    height: 100%;
  }
  .content{
    padding: 10px;
  }
}

</style>

