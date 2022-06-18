# 合約

|合約：|onWeb()|
|------:|----|
|操作：|onWeb()
交互參照：|使用案例- 註冊作業
前置條件：|存在SignUpPage頁面
後置條件：|- 建立物件SpotifySingUpPage<br>-回傳物件SpotifySingUpPage

|合約：|onSignUpClick()|
|------:|----|
|操作：|onSignUpClick()
交互參照：|使用案例- 註冊作業
前置條件：|開啟SpotifySignUpPage物件
後置條件：|- 建立類別Spotify_input的實例inputformat<br>-回傳類別Spotify_input

|合約：|SpotifySignUpClick()|
|------:|----|
|操作：|SpotifySignUpClick()
交互參照：|使用案例- 註冊作業
前置條件：|開啟inputformat()
後置條件：|- 回傳類別Spotify_input的實例inputformat

|合約：|inputformat()|
|------:|----|
|操作：|inputformat(email,username,birth,notice,passwd)
交互參照：|使用案例- 註冊作業
前置條件：|存在類別input之實例addinput
後置條件：|- 建立類別userinput的實例inputformat<br>- 實例birth與notice<br>- 實例email,username,passwd存入類別DB的實例Count_info<br>- 回傳實例inputformat

|合約：|SearchPageClick()|
|------:|----|
|操作：|SearchPageClick()
|交互參照：|使用案例- 搜尋功能
|前置條件：|存在類別Homefunction的類別Search
|後置條件：|- 建立類別Search的物件Searchinput與musictype<br>- 回傳物件Searchinput與Musictype|

|合約：|Searchfunction()|
|------:|----|
|操作：|searchfunction(searchinput,seemusictype)|
|交互參照：|使用案例- 搜尋功能
|前置條件：|存在類別Search
|後置條件：|- 建立類別Search的物件searchinput<br>- 使用物件searchinput與musictype<br>- 給定searchinput資料起始值為空白，musictype起始值為True<br>- 回傳searchinput

|合約：|SearchClick()|
|------:|----|
|操作：|SearchClick()|
|交互參照：|使用案例- 搜尋功能
|前置條件：|存在類別Search
|後置條件：|- 建立類別DB的實例searchDB<br>- 根據searchinput讀取到類別DB的實例searchDB，musictype讀取到SystemDB<br>- 回傳實例searchDB與SystemDB


|合約：|onSingInClick()|
|------:|----|
|操作：|onSingInClick()
交互參照：|使用案例- 登入作業
前置條件：|開啟SpotifySignUpPage物件
後置條件：|- 建立物件SpotifySingUpPage<br>- 回傳物件SpotifySingUpPage


|合約：|SignInInput()|
|------:|----|
|操作：|SignInInput(email,username,passwd)
交互參照：|使用案例- 登入作業
前置條件：|存在SpotifySingInPage類別的SpotifySingInPage實例
後置條件：|- 建立類別SignIn的類別SpotifySingInPage與類別SystemSignInPage <br>-建立類別SpotifySingInPage與類別SystemSignInPage的實例email,passwd,username<br>- 回傳類別SpotifySingInPage與類別SystemSignInPage


|合約：|SpotifySignInClick()|
|------:|----|
|操作：|SpotifySignInClick()|
交互參照：|使用案例- 登入作業
前置條件：|存在類別input之實例addSigninput
後置條件：|- 建立類別userSignin的實例Signinformat<br>- 實例in_username<br>- 實例in_email與in_passwd存入類別DB的實例Count_info<br>- 回傳實例Signinformat

|合約：|go()|
|------:|----|
|操作：|go()
交互參照：|使用案例- 首頁功能
前置條件：|建立類別SpotifyPage的類別HomePage
後置條件：|- 建立類別HomePage的類別UserUI的實例Permium與CountInformation<br>- 建立類別HomePage的類別Radio<br>- 建立類別HomePage的類別Music<br>- 建立類別HomePage的類別Search<br>- 建立類別HomePage的類別MusicLike<br>- 建立類別HomePage的類別MusicMenu<br>- 回傳類別HomePage的實例SuccessHomePage

|合約：|CountClick()|
|------:|----|
|操作：|CountClick()
交互參照：|使用案例- 個人資料作業
前置條件：|使用類別UserUI的實例CountInformation
後置條件：|- 根據UserUI的實例CountInformation <br> -建立實例CountBack<br> -根據實例CountInformation修改email,gender,country,place <br> -回傳實例CountBack

|合約：|PremiumClick()|
|------|----|
|操作：|PremiumClick()
交互參照：|使用案例- 會員作業
前置條件：|使用類別UserUI的實例Permium
後置條件：|- 根據UserUI的實例Permium <br> -建立類別Pay的物件Memberpay與實例Paysuccess<br> -使用物件MemberPay <br> -回傳實例Paysuccess

|合約：|MusicClick()|
|------|----|
|操作：|MusicClick()
交互參照：|使用案例- 音樂功能
前置條件：|使用類別HomePage的類別Music
後置條件：|- 建立類別的Music的實例ReponseMusic<br>- 實例PlayClick,StopClick,ToggleClick,CycleClick<br>回傳ReponseMusic

|合約：|PlayClick()|
|------|----|
|操作：|PlayClick()
交互參照：|使用案例- 音樂功能
前置條件：|使用類別HomePage的類別Music
後置條件：|- 建立類別的Music的實例PlayClick的實例ReponsePlay<br>回傳ReponsePlay

|合約：|StopClick()|
|------|----|
|操作：|StopClick()
交互參照：|使用案例- 音樂功能
前置條件：|使用類別HomePage的類別Music
後置條件：|- 建立類別的Music的實例StopClick的實例ReponseStop<br>回傳ReponseStop

|合約：|ToggleClick()|
|------|----|
|操作：|ToggleClick()
交互參照：|使用案例- 音樂功能
前置條件：|使用類別HomePage的類別Music
後置條件：|- 建立類別的Music的實例ToggleClick的實例ReponseToggle<br>回傳ReponseToggle

|合約：|CycleClick()|
|------|----|
|操作：|CycleClick()
交互參照：|使用案例- 音樂功能
前置條件：|使用類別HomePage的類別Music
後置條件：|- 建立類別的Music的實例CycleClick的實例ReponseCycle<br>回傳ReponseCycle

|合約：|MusicMenuClick()|
|------|----|
|操作：|MusicMenuClick()
交互參照：|使用案例- 音樂收藏功能
前置條件：|使用類別HomePage的類別MusicMenuClick
後置條件：|- 建立類別的MusicMenuClick的實例MusicMenu<br>回傳MusicMenu

|合約：|DeletMusicMenuClick()|
|------|----|
|操作：|DeletMusicMenuClick()
交互參照：|使用案例- 音樂收藏功能
前置條件：|使用類別HomePage的類別DeletMusicMenuClick
後置條件：|- 建立類別的DeletMusicMenuClick的實例DeletMusicMenu<br>回傳DeletMusicMenu

|合約：|MusicLikeClick()|
|------|----|
|操作：|MusicLikeClick()
交互參照：|使用案例- 音樂收藏功能
前置條件：|使用類別HomePage的類別MusicLikeClick
後置條件：|- 建立類別的MusicLikeClick的實例MusicLike<br>回傳MusicLike

|合約：|DeletMusicLikeClick()|
|------|----|
|操作：|DeletMusicLikeClick()
交互參照：|使用案例- 音樂收藏功能
前置條件：|使用類別HomePage的類別DeletMusicLikeClick
後置條件：|- 建立類別的DeletMusicLikeClick的實例DeletMusicLike<br>-回傳DeletMusicLike

|合約：|RadioPageClick()|
|------|----|
|操作：|RadioPageClick()
交互參照：|使用案例- 電台功能
前置條件：|使用類別Homefunction的類別Search
後置條件：|- 建立類別Search的類別RadioPage的實例ReponseRadioPage<br>-回傳實例ReponseRadioPage()

|合約：|RadioClick()|
|------|----|
|操作：|RadioClick()
交互參照：|使用案例- 電台功能
前置條件：|使用類別Homefunction的類別Search
後置條件：|- 建立類別RadioPage的類別RadioClick的實例ReponseRadiosuit<br>- 實例Radiosuit<br>回傳ReponseRadiosuit

|合約：|PermissionPageClick()|
|------|----|
|操作：|PermissionPageClick()
交互參照：|使用案例- 帳號權限
前置條件：|使用類別SignIn的類別SystemSignInPage
後置條件：|- 建立類別System的物件SystemGivePermisson<br>- 建立類別System的實例ReponsePermisson<br>- 建立類別System的實例permission_revise<br>- 建立類別System的實例permission_revise的實例customer與member<br>- 回傳實例ReponsePermisson
