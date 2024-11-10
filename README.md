# Error-page
注意事項
codeでこちらを読んでください

こちらはエラーページで使いやすくしました。
はじめにファイル名をerrorにしてください。

.htaccessを一番最初のページにおいてください。


構造
○○.com
  ├──index.html
  ├──style.css
  ├──.htaccess
  └──error
    ├──401.html
    ├──403.html
    ├──404.html
    └──500.html
このようにお使いください。

新しく作成するときは
CTRL+Fで変更を探してください。
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>変更</title>
    <style>
      html,body,h1,p {
        margin: 0;
        padding: 0;
      }

      body,html {
        height: 100%;
        text-align: center;
        font-family: 'ヒラギノ角ゴ Pro W3', 'Hiragino Kaku Gothic ProN', Meiryo, 'MS PGothic', Arial, sans-serif;
        background: #fafbfd;
        color: #505254;
      }

      .container {
        padding: 100px 30px;
      }

      .message {
        margin: 20px 0;
        font-size: 20px;
        line-height: 160%;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <svg xmlns="http://www.w3.org/2000/svg" width="74" height="75" viewBox="0 0 74 75"><style type="text/css">.st0{fill:#E2E8EE;}</style><path class="st0" d="M37.3 1.5c-19.8 0-36 16.1-36 36 0 19.8 16.1 36 36 36 19.8 0 36-16.1 36-36 0-19.8-16.1-36-36-36zm-29.3 36c0-6.9 2.4-13.2 6.4-18.2l41.2 41.2c-5 4-11.3 6.4-18.2 6.4-16.2-.1-29.4-13.2-29.4-29.4zm52.3 18.2l-41.2-41.1c5-4 11.3-6.4 18.2-6.4 16.2 0 29.3 13.1 29.3 29.3 0 6.9-2.4 13.2-6.3 18.2z"/></svg>
      <h1 class="message">変更</h1>
      <p>変更</p>
    </div>
  </body>
</html>

こちらは下に伸ばして使用してください。
ErrorDocument 変更 /error/変更.html
