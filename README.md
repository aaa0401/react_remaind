# React勉強
haven't I made it obvious?

# 概念
- リアクティブプログラミング：必要最低限とか時間型の変数とかいろいろ言われてる。**まともな説明がほとんどない**。
- ビルド：動かすためのコードを作ること
- イジェクト：完全に独立したアプリケーションとしてエクスポートすること
- DOM：jsからHTMLを見るときのオブジェクトのこと
- エレメント：\<p\>タグなど
- ノード：\<p\>content\</p\>の\<p\>など
- JSX：HTMLを直接jsに記述できる。書き方がより簡単になる

# よく使う記述
- ```let Dom = document.querySelector('#id');```
- ```let el1 = React.createElement(タグ, 属性, 内容);```  
  ```React.createElement('p', {}, 'aaaaaa');```など
- ```ReactDOM.render(el1, Dom);```
- ```<script src="./同ディレクトリ内.js"></script>```

# JSX
```HTML
<script src="https://unpkg.com/babel-standalone@6.26.0/babel.js"></script>
<script type="text/babel">
let el1 = {
  <div>
    <h1>This is JSX</h1>
    <p>showing how JSX works</p>
  </div>
  };
</script>
```
タグの内容に変数を用いる  ```<h1>{変数名}</h1>```  
属性に変数を用いる　```<a href={変数名}></a>```  
スタイルの場合は```{fontSize:"10pt", color:...}```のように複数指定可能  
関数の返り値も\{\}で囲んで使える  
条件でタグを追加```{ブール && タグ}```  
三項演算子版```{ブール ? 真のタグ : 偽のタグ}```  
\<li\>タグは配列で用意しておけば```{配列名}```で簡単に並べて表示できる  

ここでタグタグ叫んでいるが、タグのような形をしているだけでこれこそがJSXオブジェクト

# よく使うコマンド
- ```npx create-react-app プロジェクト名```  
- ```npm start```
