<template >
  <div>
    <div class="progres-bar">
      <div class="progres-inner">
        <span>0%</span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
 nema:'CompProgresbar'
}
</script>
<style >
.progres-bar{
  width: 100%;
  height: 20px;
  background: #fff;
  position: relative;
}
.progres-inner{
 height: 100%;
 background: linear-gradient(to right,#ED008D,#2484ED);
 border-radius: 0 10px 10px 0;
}
.progres-inner span{
 position: absolute;
 top: 50%;
 left: 50%;
 transform: translate(-50%, -50%);
 font-size: 14px;
}
</style>
