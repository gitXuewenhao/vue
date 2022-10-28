<template>
<div class="">
  <div class="block">
    <span class="demonstration">默认 Hover 指示器触发</span>
    <el-carousel height="150px">
      <el-carousel-item v-for="(item,index) in banner" :key="index">
        <h3 class="small">
          <img src="item.image" alt="">
      
        </h3>
      </el-carousel-item>
    </el-carousel>
    
  </div>
  
</div>
</template>
<script>
export default {
  data(){
    return {
      // imgUrl:"/src/assets/",
      banner:[
        {image:"/src/assets/4.jpg"},
        {image:"/src/assets/5.jpg"},
        {image:"/src/assets/6.jpg"},
        {image:"/src/assets/7.jpg"}

      ]
    }
  }
}
</script>
<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
  }

  .el-carousel__item:nth-child(2n) {
     background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
     background-color: #d3dce6;
  }
</style>