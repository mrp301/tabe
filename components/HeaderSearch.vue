<template>
  <div class='search-container'>
    <div class='logo'><a class='logo-img' href=''></a></div>
    <div class='search'>
      <input class='search-text' type='text' placeholder='エリア・駅[例：銀座、渋谷]'>
      <input class='search-text' type='text' placeholder='キーワード[例：焼肉、店名、個室]'>
      <input class='search-date' type='text' value='2018/11/17(土)'>
      <select class='search-human'>
        <option>2名</option>
        <option>3名</option>
        <option>4名</option>
        <option>5名</option>
        <option>6名</option>
        <option>7名</option>
        <option>8名</option>
        <option>9名</option>
        <option>10名</option>
      </select>
      <select class='search-time'>
        <option>13:00</option>
        <option>14:00</option>
        <option>15:00</option>
        <option>16:00</option>
        <option>17:00</option>
        <option>18:00</option>
        <option>19:00</option>
        <option>20:00</option>
        <option>21:00</option>
        <option>22:00</option>
        <option>23:00</option>
        <option>24:00</option>
      </select>
      <button class='search-btn' type='submit'></button>
    </div>
  </div>
</template>

<style lang='scss' scoped>
.search-container {
  display: flex;
  margin: 0 auto;
  padding: 10px 0;
  width: 960px;

  .logo {
    width: 150px;
    padding: 4px 0;

    .logo-img {
      display: inline-block;
      width: 130px;
      height: 26px;
      background: url('../assets/images/logo/logo_tabelog.svg');
      background-size: 130px 26px;
    }
  }

  .search {
    display: flex;
    width: 830px;

    & > input,
    & > select {
      border-top: solid 1px #eeece4;
      border-left: solid 1px #eeece4;
      border-bottom: solid 1px #eeece4;
      padding: 8px;

      &:focus {
        background: #fefae6;
      }

      &:first-child {
        border-radius: 3px 0 0 3px;
      }
    }

    .search-text {
      width: 248px;
      &:-webkit-input-placeholder {
        color: red;
      }
    }

    .search-date {
      width: 130px;
    }

    .search-human {
      width: 62px;
    }

    .search-time {
      width: 90px;
    }

    .search-btn {
      width: 5.5%;
      border: solid 1px #f3980a;
      border-radius: 0 3px 3px 0;
      cursor: pointer;
      background-image: linear-gradient(to bottom, #fa0, #f3980a);

      &:hover {
        background-image: linear-gradient(to bottom, #ffc12a, #fa0);
      }
    }
  }
}
</style>
