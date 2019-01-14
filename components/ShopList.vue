<template>
  <div>
    <ul>
      <li class='shopList'>
        <div class='shopList-header'>
          <a class='shopList-name' href=''>赤坂　ごだいご</a>
          <span class='shopList-genre'>居酒屋、おでん、焼き鳥</span>
        </div>

        <div class='shop'>
          <div class='shop-img-container'>
            <div class='shop-img'><img src='../assets/images/shopList/1.jpg'></div>
            <ul class='shop-thumbnail'>
              <li class='shop-thumbnail-item'><img src='../assets/images/shopList/detail1.jpg'></li>
              <li class='shop-thumbnail-item'><img src='../assets/images/shopList/detail1.jpg'></li>
              <li class='shop-thumbnail-item'><img src='../assets/images/shopList/detail1.jpg'></li>
              <li class='shop-thumbnail-item'><img src='../assets/images/shopList/detail1.jpg'></li>
              <li class='shop-thumbnail-item'><img src='../assets/images/shopList/detail1.jpg'></li>
            </ul>
          </div>
          <div class='shop-body'>
            <!-- ディスクリプション -->
            <div class='l-bottom-midium'>
              <div class='shop-data'>
                <div class='shop-copy'>ハイボール100円、プレミアム生350円、京風おでん、炭火焼、鮮魚が自慢。ご予約はお電話で</div>
              </div>
              <div>ネット予約で貯まる・使える</div>
            </div>

            <div class='l-bottom-xsmall'>
              <div class='shop-rate'>
                <ul class='shop-rate-star'>
                  <li><img src='../assets/images/shopList/star-enable.png'></li>
                  <li><img src='../assets/images/shopList/star-enable.png'></li>
                  <li><img src='../assets/images/shopList/star-enable.png'></li>
                  <li><img src='../assets/images/shopList/star-disable.png'></li>
                  <li><img src='../assets/images/shopList/star-disable.png'></li>
                </ul>
                <span class='shop-score'>3.52</span>
                <span class='shop-reviewCount'><a href=''>66件</a></span>
              </div>
            </div>

            <div class='l-bottom-midium'>
              <span class='shop-budget'><span class='shop-budget-night'></span>¥3,000 ~ ¥3,999</span><span class='shop-budget'><span class='shop-budget-morning'></span>-</span>
            </div>

            <ul class='shop-kwd l-bottom-midium'>
              <li>個室</li><li>全席喫煙可</li><li>飲み放題</li><li>クーポン</li>
            </ul>

            <div class='shop-pickupReview-container'>
              <a class='shop-pickupReview' href=''>
                <p class='l-bottom-small'><span class='shop-pickupReview-title'>赤坂で絶対に外さない、いや外せないお店</span><span class='shop-pickupReview-writer'>by 白ひげ海賊団(946)</span></p>
                <p>とりあえずハイボールとどんぺい焼きを！　赤坂には美味しそうな、美味しいお店がたくさんある。　それなりにコスト上がるけど美味しいお店や新店等選べない。</p>
              </a>
            </div>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<style lang='scss' scoped>

.shopList {
  border-top: solid 2px #e1e1e1;

  &:last-child {
    border-bottom: solid 2px #e1e1e1;
  }

  .shopList-header {
    padding: 13px 10px;
    border-bottom: solid 1px #e1e1e1;
  }

  .shopList-name {
    position: relative;
    display: inline-block;
    padding-left: 12px;
    font-size: 16px;
    line-height: 1.5;
    color: #0066cc;
    font-weight: bold;

    &::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 3px;
      height: 100%;
      background: #e1e1e1;
    }
  }

  .shop {
    display: flex;
    padding: 10px 10px 12px;

    .shop-img-container {
      margin-right: 12px;

      .shop-img {
        border: solid 1px #e1e1e1;
        padding: 4px;
        margin-bottom: 5px;
        width: 160px;
        height: 160px;

        * > img {
          line-height: 0;
          margin: 0;
          padding: 0;
        }
      }
    }

    .shop-thumbnail {
      display: flex;

      .shop-thumbnail-item {
        width: 28px;
        height: 28px;

        &:not(last-child) {
          margin-right: 5px;
        }

        & > img {
          width: 100%;
        }
      }
    }

    .shop-copy {
      color: #797152;
      font-weight: bold;
      line-height: 1.5;
    }

    .shop-rate {
      display: flex;
      align-items: center;

      .shop-rate-star {
        display: flex;
        margin-right: 4px;

        li {
          width: 18px;
          height: 18px;

          & > img {
            width: 100%;
          }
        }
      }

      .shop-score {
        font-size: 20px;
        font-weight: bold;
        margin-right: 14px;
      }

      .shop-reviewCount {
        position: relative;
        font-size: 14px;
        font-weight: bold;
        text-decoration: underline;
        padding-left: 20px;

        & > a {
          color: #131313;
        }

        &::before {
          position: absolute;
          left: 0;
          top: 50%;
          transform:translateY(-7px);
          content: '';
          display: inline-block;
          background-image: url('~assets/images/shopList/reviewBalloon.png');
          width: 14px;
          height: 14px;
        }
      }
    }

    .shop-budget {
      font-size: 12px;

      &:not(:last-child) {
        margin-right: 9px;
      }

      .shop-budget-night {
        vertical-align: middle;
        margin-right: 5px;

        &::before {
          content: '';
          display: inline-block;
          width: 12px;
          height: 12px;
          margin-right: 4px;
          background: url('~assets/images/moon-icon.png');
          background-size: contain;
        }
      }

      .shop-budget-morning {
        vertical-align: middle;
        margin-right: 5px;

        &::before {
          content: '';
          display: inline-block;
          width: 12px;
          height: 12px;
          margin-right: 4px;
          background: url('~assets/images/morning-icon.png');
          background-size: contain;
        }
      }
    }

    .shop-kwd {
      & >li {
        display: inline-block;
        color: #797152;
        border: solid 1px #d6ceb4;
        padding: 4px;

        &:not(:last-child) {
          margin-right: 5px;
        }
      }
    }

    .shop-pickupReview-container {
      padding: 12px 16px;
      background: #faf8f5;
    }

    .shop-pickupReview {
      display: block;
      color: #595960;

      &:hover {
        text-decoration: none;
      }

      .shop-pickupReview-title {
        font-weight: bold;
        border-bottom: dotted 1px;
        font-size: 12px;
        color: #13131e;
        margin-right: 6px;
        vertical-align: middle;
        line-height: 1.6;

        &:hover {
          color: #ff9600;
        }
      }

      .shop-pickupReview-writer {
        font-size: 10px;
      }
    }
  }
}

</style>
