# EmptyNodeAngular2
Empty Anggular2 ( basic structure)

此為　Anggular2　for TypeScript 的空白專案　，　請確認您已安裝　node & npm 以及全域按裝 npm tsd套件

操作步驟:

1.下載 git clone https://github.com/suntan/EmptyNodeAngular2.git 

2.修改下載資料夾名稱 , 喜歡的名稱就OK　；　以下　MyProject　作為新資料夾名稱

[root@/usr/src]# mv EmptyNodeAngular2 MyProject

3.切換目錄至 MyProject 之下

[root@/usr/src]# cd MyProject

4.修改　package.json 中的檔案名稱為上述 [資料夾名稱(MyProject)]

[root@/usr/src/MyProject]# vi package.json

{

  "name": "EmptyNodeAngular2", <---- 專案名稱 , 修改為 [資料夾名稱(MyProject)]
  
  "version": "1.0.0",
  
  "scripts": {
  
    "start": "concurrently \"npm run tsc:w\" \"npm run lite\" ",    
    
    "tsc": "tsc",
    
    "tsc:w": "tsc -w",
    
    "lite": "lite-server",
    
    "typings": "typings",
    
    "postinstall": "typings install" 
    
  },
  
  "license": "ISC",
  
  "dependencies": {
  
    "angular2": "2.0.0-beta.13",
    
    "systemjs": "0.19.25",
    
    "es6-shim": "^0.35.0",
    
    "reflect-metadata": "0.1.2",
    
    "rxjs": "5.0.0-beta.2",
    
    "zone.js": "0.6.6"
    
  },
  
  "devDependencies": {
  
    "concurrently": "^2.0.0",
    
    "lite-server": "^2.1.0",
    
    "typescript": "^1.8.9",
    
    "typings":"^0.7.11"
    
  }
  
}

修改如下:

{

  "name": "MyProject", <---- 專案名稱 , 修改為 [資料夾名稱(MyProject)]
  
  "version": "1.0.0",
  
  "scripts": {
  
    "start": "concurrently \"npm run tsc:w\" \"npm run lite\" ",    
    
    "tsc": "tsc",
    
    "tsc:w": "tsc -w",
    
    "lite": "lite-server",
    
    "typings": "typings",
    
    "postinstall": "typings install" 
    
  },
  
  "license": "ISC",
  
  "dependencies": {
  
    "angular2": "2.0.0-beta.13",
    
    "systemjs": "0.19.25",
    
    "es6-shim": "^0.35.0",
    
    "reflect-metadata": "0.1.2",
    
    "rxjs": "5.0.0-beta.2",
    
    "zone.js": "0.6.6"
    
  },
  
  "devDependencies": {
  
    "concurrently": "^2.0.0",
    
    "lite-server": "^2.1.0",
    
    "typescript": "^1.8.9",
    
    "typings":"^0.7.11"
    
  }
  
}


5.下 npm install 指令進行 node_modules 安裝

6.開始在 app 資料夾下的 Entry point main.ts & app.component.ts 加菜吧~~~
