# Wordle Solver

## 必備軟體
* 支援C++17的編譯器

## 開始

### 下載程式碼

#### 由git clone指令下載
`git clone https://gitlab.com/ryanovovo/wordle-
solver.git`

#### 由連結下載
[Link](https://gitlab.com/ryanovovo/wordle-solver/-/archive/master/wordle-solver-master.zip)

### 進入目錄
`cd wordle-solver`

### 更改檔案路徑
#### 將程式中186及187行的檔案路徑更改為自己的檔案路徑
`ifstream words ("/Users/ryanovovo/Documents/GitHub/wordle-solver/words.txt");`

改為

`ifstream words ("YOUR_DIRECTORY/words.txt");`


`ifstream diff  ("/Users/ryanovovo/Documents/GitHub/wordle-solver/all_words_diff.txt");`

改為

`ifstream diff  ("YOUR_DIRECTORY/all_words_diff.txt");`



### 編譯程式碼
#### 使用指令
```
g++ -o wordle_solver wordle_solver.cpp
```

### 執行程式
`./wordle_solver`


## 程式使用說明

### 選擇wordle的困難度
wordle有提供兩種遊戲模式，normal(預設) hard(要去設定中打開)
![](https://i.imgur.com/PljMVCf.png)

#### 初始化完畢後選擇困難度

* `n` = 普通模式
* `h` = 困難模式


### 選擇執行模式
執行模式分為解決模式和測試模式
* `s` = 解決模式
* `t` = 測試模式

解決模式為一般使用，測試模式為統計程式執行的效果

選擇`s` 一般模式即可

### 輸入執行結果
螢幕會印出程式運算後最佳的猜測結果，將程式得出的最佳猜測結果輸入至wordle遊戲中

wordle遊戲的回傳結果請依照下方圖示填入程式中

🟩 = `o`

🟨 = `_`

⬛ = `x`

填入後按下`enter`鍵，程式會自動印出下一個最佳猜測的單字

請繼續輸入直到猜中為止

**注意！！** 

猜中後程式會自動執行下一輪新的猜測，若要退出請按`ctrl+c`


### Demo影片

[<img alt="Wordle Solver Demo" width="400px" src="https://i.imgur.com/VeRcmb7.png" />](https://www.youtube.com/watch?v=6ePgQ4rbVAo)










