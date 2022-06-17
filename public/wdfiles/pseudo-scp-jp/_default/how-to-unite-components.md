---
title: "如何にしてコンポーネントをまとめるか"
createdBy: "RTa_technology"
originUrl: "http://pseudo-scp-jp.wikidot.com/how-to-unite-components"
tags: ["エッセイ", "rta-technology"]
---
[[toc]]
+ 前置き
自作の構文を作るとき，includeするべきページがどんどん増えていくことがあるのではないかと思います．
[[div class="code"]]
@@[@@[include [# :ooo:---:xxx-top]]]
= [中略]
@@[@@[include [# :ooo:---:xxx-mid]]]
= [中略]
@@[@@[include [# :ooo:---:xxx-end]]]

途中で，@@[@@[include [# :ooo:---:xxx-mid2]]]を入れる……
[[/div]]
みたいな経験はありませんか?
もしくは，
[[div class="code"]]
@@[@@[include [# :ooo:---:xxx]]]
@@ \_[@@[include [# :ooo:---:xxx-base]]]
@@    \_@@[[include [# :ooo:---:xxx-base2]]]
[[/div]]といった具合に内包関係であったり．
作るときは楽ですが，いざ使うとなったら(何も考えずに使う側はそのままコピーすればいいですが)includeすべきページがたくさんあってとても紛らわしいことこの上ないでしょう．
その為，今回は2つほどそれらの紛らわしい悩みを解決できる方法をご紹介しようと思います．