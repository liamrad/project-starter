<template>
  <div class="components_base-side-routes">
    <el-menu router>
      <el-menu-item
        v-for="route in $router.options.routes"
        :key="route.path"
        :index="route.path"
        :route="route"
      >
        <span class="singal-row-ellipsis">{{ route.path }}</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<style scoped>
.components_base-side-routes {
  height: 100%;
  overflow: auto;
}
</style>
