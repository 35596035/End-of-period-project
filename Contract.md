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
|合約：|SearchPageClick()|
|------|----|
|操作：|SearchPageClick()
|交互參照：|使用案例-搜尋功能
|前置條件：|存在類別Homefunction的實例Search
|後置條件：|建立類別Search的物件Searchinput與musictype
||-回傳物件Searchinput與Musictype|

|合約：|Searchfunction()|
|------|----|
|操作：|searchfunction(searchinput,seemusictype)|
|交互參照：|使用案例-搜尋功能
|前置條件：|存在類別Search
|後置條件：|-建立類別Search的物件SearchInput
||-使用物件searchinput與musictype
||-給定searchinput資料起始值為空白，musictype起始值為True
||-根據searchinput讀取到類別DB的實例searchDB，musictype讀取到SystemDB
||-回傳實例searchDB與SystemDB

|合約：|SearchClick()|
|------|----|
|操作：|SearchClick()|
|交互參照：|使用案例-搜尋功能
|前置條件：|存在類別Search
|後置條件：|-將Searchmusic存入Searchresuit
||-根據Searchresuit讀取SearchDatabase|
||-回傳Search|


|合約：|onSingInClick()|
|------|----|
|操作：|onSingInClick()
交互參照：|使用案例- 登入作業
前置條件：|存在SpotifySingInPage頁面
後置條件：|-建立物件onSingIn


|合約：|SignInInput()|
|------|----|
|操作：|SignInInput()(email,username,passwd)
交互參照：|使用案例- 登入作業
前置條件：|存在SpotifySingInPage類別的SpotifySingInPage實例
後置條件：|-將輸入的email,username,passwd


|合約：|SpotifySignInClick()|
|------|----|
|操作：|SpotifySignInClick()|
交互參照：|使用案例- 登入作業
前置條件：|存在SpotifySingInPage頁面
後置條件：|-
