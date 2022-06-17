# 合約

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