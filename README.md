### 参考

https://www.youtube.com/watch?v=8UVRsJnD3Cc

### Commands

コンテナ内の bash に入る  
`docker-compose exec front sh`

### 環境構築

`npx create-react-app . --template typescript --use-npm`

#### eslint

`npx eslint --init`
`npm i -D eslint-plugin-jest`

#### prettier

https://qiita.com/park-jh/items/c31784c950561521d035
`npm i -D prettier eslint-config-prettier eslint-plugin-prettier pretty-quick`

#### lint 実行

`npm run lint`

#### docker-compose build

エラーが発生した時はエラーメッセージに従ってみる。

- package.json の下記バージョンをエラーメッセージ記載のバージョンに修正
  "devDependencies": {
  "eslint": "^6.6.0"
  }

docker-compose run --rm front sh
npm install
