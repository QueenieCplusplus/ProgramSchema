# ProgramSchema
編程機制

撰寫程式碼前，需要了解電腦自身的作業環境(亦稱平台)，以及使用何種編譯器。

# 程式碼機制運作的流程圖

                      Source Code
                      
                           |
                           V
                       
    after process of Compiling | Interpreting | TransCompiling
    
                     Build | Make (options)
    
                           |
                           V
                           
                      Object Code
                      
                           |
                           V
                           
              after process of Loader & Linker
              
        (then link with std lib and generate start code)
        
                           |
                           V
                        
                     Excutable Code
                     
                           |
                           V
                           
                       Run | Debug (options)
                     

# 檢視步驟

＊ 使用文字編輯器編輯程式碼，成為所謂的 Src Code 源碼。

＊ 腳本語言透過直譯，而強型別語言均需要透過編譯或轉譯成為機器碼 Machine Code，以及另外一份稱為目的地碼 Object Code 的檔案。

＊ 利用 Loader & Linker 結合語言自身的標準函數庫 stardard Lib，而 C++ 函數庫是含有一群稱為 function 的電腦 routine 的目的地碼，Linker 動作本身並非單純組合目的地碼，還會加入 Startup Code 啟動碼，產生 Runtime Version，並且將產生 Excutable Code (常常聽見的可執行檔)。

# 編譯與組建的分別

* complie: 僅編譯目前開啟的源碼。

* build: 編譯專案所有的源碼。

# 可選步驟

* Run：完成所有上述過程，並且執行。

* Debug：完成所有上述過程，並且逐一執行。

