<script lang="ts" setup>
// 页脚需要的链接
const links = {
    ShijieLian: "https://github.com/LiamLian0727"
}
</script>

<template>
  
  <div class="bg">
    
    <el-watermark :content="['Euclid\'s Gift', 'ZGCA', 'ZGCAI']" :gap="['60','0']" :z-index="0">
      <el-row justify="center">
        <p class="footer">
          This page was primarily created by <a :href="links.ShijieLian">Shijie Lian</a>.
        </p>
      </el-row>
    </el-watermark>
  </div>
</template>

<style scoped>

/* 页脚背景 */
.bg {
  background-color: rgb(235, 235, 235);
}

/* 页脚文字 */
.footer {
  text-align: center;
  margin: 20px;
  z-index: 1;
}

</style>