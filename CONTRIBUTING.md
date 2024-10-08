## Environment Installation 環境安裝
- #### Install CPython (the official Python) 3.11 or higher.<br/>安裝 CPython（官方版本的 Python）3.11 或更高版本。
  You can find it on <https://www.python.org/>.<br/>
  可至 <https://www.python.org/> 下載。
- #### Install requirements.<br/>安裝依賴套件。
  Download [requirements.txt](requirements.txt) and run the following command:<br/>
  下載 [requirements.txt](requirements.txt) 並執行以下命令：
  
  ```
  pip install -r requirements.txt
  ```
## Project Structure 專案架構
```py
GameCorner/
│
├── GameCorner.py  # the entry point of the program  # 程式的進入點
├── load_env.py  # load the .env file  # 載入 .env 檔
├── games.py  # the code about loading game files  # 用於載入遊戲的程式碼
├── users.py  # the code that controls things about users  # 跟使用者有關的程式碼
├── utils.py  # other functions  # 其他函數
├── Renderer.py  # to render the game HTML  # 用於將遊戲程式的入口檔和依賴資源組裝起來的渲染器
├── .env  # your environment variable file (we do not provide, but it should be placed here)
│         # 您的環境變數檔（我們沒有提供，但它應該放在這裡）
├── templates/  # HTML templates  # HTML 模板
│    ├── index.html  # home page  # 首頁
│    ├── game.html  # game page for each game  # 個別遊戲的遊戲頁面
│    └── myCreation.html  # page for game developers to manage their games  # 讓遊戲開發者管理遊戲的頁面
├── static/  # static resources  # 靜態資源
│    └── GameCorner.ico  # Favicon
└── src/  # the place for images or something else  # 放圖片和其他東西的地方
    └── ...
```

## Docs 相關文件
See documents in "[docs](./docs)" folder to learn more about this project.<br/>
參考「[docs](./docs)」資料夾中的文件來了解更多關於本專案的細節。

## TODO
- [x] Load game files through database API. 透過資料庫的 API 讀取遊戲檔案。
- [x] The game page. 遊戲頁面。
- [ ] A page for game producers to manage games and upload game files. 遊戲檔案的管理和上傳頁面。
  - [ ] 前後端資料串接
    - [ ] 查詢
    - [ ] 上傳
    - [ ] 更新
    - [x] 刪除
