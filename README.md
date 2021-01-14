# Open APIの定義について

## 導入手順
1. yamlファイルでAPI設計を記述する
   1. 記載方法は、`https://github.com/swagger-api/swagger-editor`のルートにある`index.html`を参照
1. VSCodeに`Swagger Viewer`の拡張を導入する
1. VSCodeで`Shift + Option + P`を押すと、プレビューが確認できる

## 困りごと
* `npm start`してもローカルサーバーが起動できない（ログは以下の通り）
```
> shop-review-api@1.0.0 prestart /Users/mikaurakawa/Desktop/personal_learning/nodejs-server-server-generated
> npm install

audited 107 packages in 1.559s

2 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities


> shop-review-api@1.0.0 start /Users/mikaurakawa/Desktop/personal_learning/nodejs-server-server-generated
> node index.js

body-parser deprecated undefined extended: provide extended option node_modules/oas3-tools/dist/middleware/express.app.config.js:22:33
  Mock mode: disabled
/Users/mikaurakawa/Desktop/personal_learning/nodejs-server-server-generated/index.js:15
expressAppConfig.addValidator();
                 ^

TypeError: expressAppConfig.addValidator is not a function
    at Object.<anonymous> (/Users/mikaurakawa/Desktop/personal_learning/nodejs-server-server-generated/index.js:15:18)
    at Module._compile (internal/modules/cjs/loader.js:1200:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:1220:10)
    at Module.load (internal/modules/cjs/loader.js:1049:32)
    at Function.Module._load (internal/modules/cjs/loader.js:937:14)
    at Function.executeUserEntryPoint [as runMain] (internal/modules/run_main.js:71:12)
    at internal/main/run_main_module.js:17:47
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! shop-review-api@1.0.0 start: `node index.js`
npm ERR! Exit status 1
npm ERR! 
npm ERR! Failed at the shop-review-api@1.0.0 start script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/mikaurakawa/.npm/_logs/2020-12-25T04_18_05_367Z-debug.log
```# openapi-learning
