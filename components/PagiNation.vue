<template>
  <div class='pagiNation-container'>
    <ul class='pagiNation'>
      <li class='pagiNation-previous'><a href=''>前の20件</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>1</a></li>
      <li class='pagiNation-item pagiNation-item-active'><a class='pagiNation-link' href=''>2</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>3</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>4</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>5</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>6</a></li>
      <li class='pagiNation-item none'><span>...</span></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>10</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>20</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>30</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>40</a></li>
      <li class='pagiNation-item'><a class='pagiNation-link' href=''>50</a></li>
      <li class='pagiNation-next'><a href=''>次の20件</a></li>
    </ul>
  </div>
</template>

<style lang='scss' scoped>
.pagiNation-container {
  margin-bottom: 30px;
  padding: 20px 0;
  background: #faf8f5;
  border-top: solid 1px #eeece4;
  border-bottom: solid 1px #eeece4;

  .pagiNation {
    display: flex;
    justify-content: center;

    .pagiNation-item {
      border: solid 1px #eeece4;
      background: #fff;

      &:not(first-child) {
        margin-left: -1px;
      }

      .pagiNation-link {
        display: block;
        width: 32px;
        height: 32px;
        line-height: 32px;
        text-align: center;
        text-decoration: none;
        color: #13131e;

        &:hover {
          color: #fff;
          border-color: #ff9600;
          background: #ff9600;
        }
      }

      &.none {
        border-top: none;
        border-bottom: none;

        span {
          display: block;
          width: 24px;
          height: 32px;
          line-height: 32px;
          text-align: center;
          background: #faf8f5;
        }
      }

      &.pagiNation-item-active {
        font-weight: bold;
        border-top: none;
        border-bottom: solid 2px #d6ceb4;
        background: #faf8f5;
      }
    }

    .pagiNation-previous {
      margin-right: 10px;

      a {
        display: block;
        height: 32px;
        line-height: 32px;
        font-size: 14px;

        &:hover {
          text-decoration: none !important;
        }
      }
    }

    .pagiNation-next {
      margin-left: 10px;

      a {
        display: block;
        height: 32px;
        line-height: 32px;
        font-size: 14px;

        &:hover {
          text-decoration: none !important;
        }
      }
    }
  }
}
</style>
