# 專案畫面
![image](https://github.com/yun856839/Todo-Sequelize/blob/master/todo-sequelize.jpg)
![image](https://github.com/yun856839/Todo-Sequelize/blob/master/todo-sequelize2.jpg)

# Todo-Sequelize
* 使用MySQL打造，供使用者建立個人 todo-list

# 功能描述 (features)
* 使用者可以創建帳號並登入
* 使用者可以使用 FaceBook 登入
* 使用者可以新增代辦事項
* 使用者可以瀏覽特定代辦事項
* 使用者可以修改代辦事項
* 使用者可以刪除特定代辦事項

# 環境建置與需求 (prerequisites)
* Node.js: 14.4.0
* bcryptjs: 2.4.3
* connect-flash: 0.1.1
* dotenv: 8.2.0
* express: 4.17.1
* express-session: 1.17.1
* express-Handlebars: 5.2.0
* method-override: 3.0.0
* passport: 0.4.1
* passport-facebook: 3.0.0
* passport-local: 1.0.0
* mysql2: 2.2.5,
* sequelize: 6.5.0
* sequelize-cli: 6.2.0


# 安裝與執行步驟(installation and execution)
  1. 打開終端機(Terminal)，Clone 此專案至本地電腦
  ```
  git clone https://github.com/yun856839/Todo-Sequelize.git
  ```

  2. 開啟終端機，進入專案資料夾
  ```
  cd todo-sequelize
  ```

  3. 安裝 npm 套件
  ```
  npm install
  ```
  
  4. 使用 MySQL Workbench 建立資料庫
  ```
  drop database if exists todo_sequelize;
  create database todo_sequelize;
  use todo_sequelize;
  ```
  
  5.在終端機執行：把專案裡的 migration 設定檔同步到資料庫，並執行種子資料
  ```
  npx sequelize db:migrate
  npx sequelize db:seed:all
  ```

  6. 執行 server
  ```
  npm run dev
  ```

  7. 開啟任一瀏覽器瀏覽器，輸入網址
  ```
  http://localhost:3000
  ```
