<template>
  <el-row type="flex" justify="center">
    <el-col :span="20">
    <h1>About Shop</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci, aliquid atque deserunt dicta eligendi
      excepturi expedita harum iusto laudantium maiores minima molestias natus non, quidem, quos repellendus similique
      suscipit vero?</p>
    </el-col>
  </el-row>
</template>

<script>
  export default {
    async asyncData() {
      return {
        renderSource: process.static ? 'static' : (process.server ? 'server' : 'client')
      }
    },
    methods: {
      reloadPage() {
        window.location.reload()
      }
    }
  }
</script>