<template>
  <header>
    <div class='header-container'>
      <div class='header'>
        <div class='header-left'>
          <p>全国のおでん</p>
        </div>
        <div class='header-right'>
          <ul class='header-menu'>
            <li><a href=''>食べログの特徴と便利な使い方</a></li>
            <li><a href=''>無料完飲登録</a></li>
            <li><a href=''>保有Tポイント</a></li>
            <li><a href=''>予約確認</a></li>
            <li><a href=''>行ったお店</a></li>
            <li><a href=''>保存済み</a></li>
            <li><a href=''>ログイン</a></li>
          </ul>
        </div>
      </div>
      <HeaderSearch></HeaderSearch>
    </div>
   <p>ヘッダー</p>
  </header>
</template>

<style lang='scss' scoped>
.header-container {
  border-top: solid 2px #fa0;
  box-shadow: 0 2px 2px -1px #eeece4;

  .header {
    width: 980px;
    margin: 0 auto;
    padding: 10px 0;
    display: flex;
    justify-content: space-between;

    .header-menu {
      & > * {
        display: inline-block;
        padding: 0 8px;
        color: #06c;
         a {
           text-decoration: none;

           &:hover {
             color: #ff9600;
             text-decoration: underline;
           }
         }

        &:not(:last-child) {
          border-right: solid 1px #eeece4;
        }
      }
    }
  }
}
</style>

<script>

import HeaderSearch from '~/components/HeaderSearch'

export default {
  components: {
    HeaderSearch
  }
}

</script>
