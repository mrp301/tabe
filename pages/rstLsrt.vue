<template>
  <div class='layout-container'>
    <div class='layout clearfix'>
      <div class='layout-main'>
        <p>コンテンツ</p>
        <PagiNation></PagiNation>
      </div>
      <div class='layout-side'>サイドバー</div>
    </div>
  </div>
</template>

<script>
import PagiNation from '~/components/PagiNation'

export default {
  components: {
    PagiNation
  }
}
</script>

<style lang='scss' scoped>
.layout-container {
  width: 100%;

  .layout {
    width: 980px;
    margin: 0 auto;

    .layout-main {
      float: right;
      width: 770px;
    }

    .layout-side {
      float: left;
      width: 190px;
    }
  }
}
</style>
