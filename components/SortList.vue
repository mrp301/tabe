<template>
  <div class='sortList-container'>
    <ul class='sortList'>
      <li class='sortList-item sortList-item-standard sortList-item-active'>
        <a href=''>
          <p class='sortList-item-icon sortList-item-icon-standard'>標準<span>【会員店舗優先順】</span></p>
        </a>
      </li>
      <li class='sortList-item sortList-item-ranking'>
        <a href=''>
          <p class='sortList-item-icon sortList-item-icon-ranking'>ランキング</p>
        </a>
      </li>
      <li class='sortList-item sortList-item-review'>
        <a href=''>
          <p class='sortList-item-icon sortList-item-icon-review'>口コミ数数</p>
        </a>
      </li>
      <li class='sortList-item sortList-item-new'>
        <a href=''>
          <p class='sortList-item-icon sortList-item-icon-new'>ニューオープン順</p>
        </a>
      </li>
    </ul>
  </div>
</template>

<style lang='scss' scoped>

.sortList-container {
  background: #faf8f5;
  border-bottom: solid 1px #e0dccc;
  padding: 0 20px;
  box-shadow: 0 1px 0 #eeece4 inset;

  .sortList {
    display: flex;
    margin: 0 auto;

    .sortList-item {
      width: 25%;
      padding: 13px 0;
      text-align: center;

      & > a {
        display: block;
        font-size: 13px;
        color: #463f2d;

        &:hover {
          text-decoration: none;
        }

        & > p {
          border-left: solid 1px #e0dccc;
        }
      }

      &.sortList-item-standard {

        &:hover {
          border-top: solid 1px #e06650;

           * {
            color: #e06650;
          }
        }
      }

      &.sortList-item-ranking {

        &:hover {
          border-top: solid 1px #fcb720;

           * {
            color: #fcb720;
          }
        }
      }

      &.sortList-item-review {

        &:hover {
          border-top: solid 1px #88bd2a;

           * {
            color: #88bd2a;
          }
        }
      }

      &.sortList-item-new {

        &:hover {
          border-top: solid 1px #5498cb;

           * {
            color: #5498cb;
          }
        }
      }

      .sortList-item-icon {
        line-height: 20px;

        &::before {
          content: '';
          display: inline-block;
          width: 20px;
          height: 20px;
          margin-right: 6px;
          vertical-align: bottom;
        }

        &.sortList-item-icon-standard {

          &::before {
            background: url('~assets/images/standard.png');
          }
        }

        &.sortList-item-icon-ranking {

          &::before {
            background: url('~assets/images/ranking.png');
          }
        }

        &.sortList-item-icon-review {
          &::before {
            background: url('~assets/images/review.png');
          }
        }

        &.sortList-item-icon-new {
          &::before {
            background: url('~assets/images/new.png');
          }
        }
      }

       &.sortList-item-active {
         position: relative;
         background: #fff;
         border-left: solid 1px #e0dccc;
         border-right: solid 1px #e0dccc;
         border-bottom: solid 1px #fff;
         font-weight: bold;

         & > a > p,
         & + .sortList-item > a p { /*アクティブ要素とその次の要素の区切り線を非表示にする */
           border-left: none;
         }

         &.sortList-item-standard {
           border-top: solid 1px #e06650;

           & > a {
             color: #e06650;
           }
         }

         &.sortList-item-ranking {
           border-top: solid 1px #fcb720;

           & > a {
             color: #fcb720;
           }
         }

         &.sortList-item-review {
           border-top: solid 1px #88bd2a;

           & > a {
             color: #88bd2a;
           }
         }

         &.sortList-item-new {
           border-top: solid 1px #5498cb;

           & > a {
             color: #5498cb;
           }
         }

         &::after {
           position: absolute;
           content: '';
           display: inline-block;
           left: 0;
           bottom: -2px;
           width: 100%;
           height: 1px;
           background: #fff;
         }
       }
    }
  }
}

</style>
