# タスク
- PrimeFlexのバックグラウンドカラーを使えるように調整
  - Primevueとも調整必須？
---
やったこと

# nuxt追加
- Node.js(https://nodejs.org/en) をインストール
  - npx nuxi init を起動
  - yarn(ターミナルでyarnと入力)をインストール
  - \ProgrammingLearningApp\nuxt-app> npm run dev で起動→テストが出てくればよい
    - npm run devがエラーが出る場合→packege.jsonからデバックをクリックで起動

# docsフォルダ追加
- Idea.mdにマインドマップを追記

# PrimeVue追加
UIコンポーネントが使える便利なもの
→UIの統一化が簡単なので使用したい

- npm install primevue, npm install --save-dev @primevue/nuxt-module,npm install @primevue/themes,npm install primeiconsを入れる
- runしたとき黒ボタンが出ていればOK
- [公式サイト](https://primevue.org/) 

# PrimeFlex追加
Bootstrapみたいなもの

- npm install primeflex　を入れる
- 入っているが色関係がPrimeVewと競合している気がする
- [公式サイト](https://primeflex.org/)

# componentの使用例を追加
- app.vueを親としてcomponentファイル内のsanple.vueを子コンポーネントとして使用
  - テキストボックスに入っている文字をボタンクリックしたら別の個所に表示する仕組みを分けただけ
