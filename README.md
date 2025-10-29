<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>版面配置範例</title>
  <style>
    body {
      margin: 0;
      font-family: 'Noto Sans TC', sans-serif;
      text-align: center;
    }

    header, footer {
      background-color: #fff;
      padding: 10px 0;
      font-size: 1.5em;
    }

    main {
      display: flex;
      flex-wrap: wrap;
      min-height: 80vh;
    }

    nav {
      flex: 1 1 200px;
      background-color: #ffffe0; /* 淡黃色 */
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.3em;
    }

    section {
      flex: 3 1 400px;
      background-color: #d3d3d3; /* 灰色 */
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.8em;
    }

    aside {
      flex: 1 1 200px;
      background-color: #ffb6c1; /* 粉紅色 */
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.3em;
    }

    @media (max-width: 768px) {
      main {
        flex-direction: column;
      }

      nav, aside, section {
        flex: 1 1 100%;
        min-height: 150px;
      }
    }
  </style>
</head>
<body>
  <header>首頁</header>

  <main>
    <nav>導覽列</nav>
    <section>主要內容</section>
    <aside>側邊欄</aside>
  </main>

  <footer>頁尾</footer>
</body>
</html>
