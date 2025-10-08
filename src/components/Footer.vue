<script lang="ts" setup>
// 页脚需要的链接
const links = {
    DingkunLiu: "https://github.com/Dingkun0817"
}

// 水印内容
const watermarkContent = ["MIRepNet", 'HUST', 'ZGCA']
</script>

<template>
  
  <div class="bg">
    
    <el-watermark :content="watermarkContent" :gap="['60','0']" :z-index="0">
      <el-row justify="center">
        <p class="footer">
          This page was created by <a :href="links.DingkunLiu">Dingkun Liu</a>.
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