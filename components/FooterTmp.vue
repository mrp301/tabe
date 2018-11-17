<template>
  <footer>
    <div class='footer'>
      <div class='footer-service-container'>
        <div class='footer-service'>
          <a href=''>
            <img src='../assets/images/logo/footer_tabelog_matome.gif'><br>
            <span class='footer-service-text'>グルメキュレーションサイト</span>
          </a>
        </div>
        <div class='footer-service'>
          <a href=''>
            <img src='../assets/images/logo/footer_tabelog_magazine.gif'><br>
            <span class='footer-service-text'>毎日の外食が楽しくなるグルメ情報</span>
          </a>
        </div>
        <div class='footer-service'>
          <a href=''>
            <img src='../assets/images/logo/logo_reviewer_ranking.svg' width='158' height='24'><br>
            <span class='footer-service-text'>全国で活躍するレビュアー</span>
          </a>
        </div>
      </div>

      <div class='footer-nav-container'>
        <div class='footer-nav'>
          <ul>
            <li><a href=''>ヘルプ・お問い合わせ</a><span>|</span></li>
            <li><a href=''>食べログの特徴と便利な使い方</a><span>|</span></li>
            <li><a href=''>口コミ・ランキングに対する取り組み</a><span>|</span></li>
            <li><a href=''>FAQ</a></li>
            <li><a href=''>集客サービス（飲食店・飲食店企業様向け）について</a><span>|</span></li>
            <li><a href=''>広告（メーカー・団体様等向け）について</a><br></li>
            <li><a href=''>機能改善要望</a><span>|</span></li>
            <li><a href=''>口コミガイドライン</a><span>|</span></li>
            <li><a href=''>プレミアムサービス</a><span>|</span></li>
            <li><a href=''>プレミアムサービス無料クーポン</a><span>|</span></li>
            <li><a href=''>ワンコインランチクーポン（無料体験）</a><span>|</span></li>
            <li><a href=''>利用規約</a><span>|</span></li>
            <li><a href=''>個人情報保護方針</a><span>|</span></li>
            <li><a href=''>企業情報</a><span>|</span></li>
            <li><a href=''>サイトマップ</a><br></li>
            <li><a href=''>キーワード一覧</a><span>|</span></li>
            <li><a href=''>チェーン店一覧</a></li>
          </ul>
        </div>
      </div>

      <div class='footer-language-container'>
        <div class='footer-language'>
          <span class='footer-language-title'>言語 ： </span>
          <ul>
            <li><a href=''>English</a></li>
            <li><a href=''>简体中文</a></li>
            <li><a href=''>繁體中文</a></li>
            <li><a href=''>한국어</a></li>
          </ul>
        </div>
      </div>

      <div class='footer-copyright-container'>
        <div class='footer-copyright'>
          <a class='footer-copyright-logo' href=''></a>
          <small class='footer-copyright-text'><p>Copyright (c) Kakaku.com, Inc. All Rights Reserved. 無断転載禁止</p></small>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang='scss' scoped>
.footer {
  width: 100%;

  .footer-service-container {
    display: flex;
    width: 980px;
    margin: 0 auto;
    padding: 20px 0;
    justify-content: center;

      a {
        display: block;
        text-decoration: none;
      }

    .footer-service {
      width: 326px;
      text-align: center;
      border-right: 1px solid #eeece4;

      &:last-child {
        border-right: none;
      }

      .footer-service-text {
        color: #959599;
        font-size: 10px;

        &:hover {
          color: #959599;
          text-decoration: underline;
        }
      }
    }
  }

  .footer-nav-container {
    background: #faf8f5;
    padding: 22px 0;

    .footer-nav {
      margin: 0 auto;

      ul {
        text-align: center;

        li {
          display: inline;
          line-height: 2;

          a {
            color: #06c;
            text-decoration: none;
            font-size: 10px;

            &:hover {
              color: #ff9600;
              text-decoration: underline;
            }
          }

          span {
            padding: 0 4px;
            color: #d0d0d0;
          }
        }
      }
    }
  }

  .footer-language-container {
    border-bottom: solid 1px #eeece4;

    .footer-language {
      width: 980px;
      margin: 0 auto;
      padding: 30px 0;
      display: flex;
      justify-content: center;

      .footer-language-title {
        color: #949499
      }

      ul {
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

  .footer-copyright-container {
    .footer-copyright {
      width: 980px;
      margin: 0 auto;
      padding-top: 15px;
      display: flex;
      justify-content: space-between;

      .footer-copyright-logo {
        display: inline-block;
        width: 96px;
        height: 20px;
        background: url('../assets/images/logo/logo_tabelog.svg');
        background-size: 96px 20px;
      }

      .footer-copyright-text {
        color: #949499;
        justify-content: flex-end;
      }
    }
  }
}
</style>
