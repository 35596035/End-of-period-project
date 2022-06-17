# 合約

|合約：|onWeb()|
|------|----|
|操作：|onWeb()
交互參照：|使用案例-註冊作業
前置條件：|存在SignUpPage頁面
後置條件：|- 建立物件SpotifySingUpPage<br>-回傳物件SpotifySingUpPage

|合約：|onSignUpClick()|
|------|----|
|操作：|onSignUpClick()
交互參照：|使用案例-註冊作業
前置條件：|開啟SpotifySignUpPage物件
後置條件：|-建立類別Spotify_input的實例inputformat<br>-回傳類別Spotify_input

|合約：|SpotifySignUpClick()|
|------|----|
|操作：|SpotifySignUpClick()
交互參照：|使用案例-註冊作業
前置條件：|-使用inputformat()
後置條件：|-回傳類別Spotify_input的實例inputformat

|合約：|inputformat()|
|------|----|
|操作：|inputformat(email,username,
birth,notice,passwd)
交互參照：|使用案例-註冊作業
前置條件：|存在類別input之實例addinput
後置條件：|-建立類別userinput的實例inputformat<br>-實例,birth與notice<br>-實例email,username,passwd存入類別DB的實例Count_info<br>-回傳實例inputformat

|合約：|go()|
|------|----|
|操作：|go()
交互參照：|使用案例-首頁功能
前置條件：|-建立類別SpotifyPage的類別S_HomePage
後置條件：|-