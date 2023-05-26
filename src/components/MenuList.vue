<template>
  <el-menu
    default-active="/"
  >
    <el-menu-item v-for="item in menuList" :index="item.path" :key="item.path" @click="changePath(item.path)">
      <el-icon>
        <component :is="item.icon"></component>
      </el-icon>
      <span>{{item.name}}</span>
    </el-menu-item>
  </el-menu>
</template>

<script setup>
import menuList from '../assets/menuList';
import { useRouter } from 'vue-router';

const router = useRouter();
function changePath (path) {
  router.push(path);
}

</script>