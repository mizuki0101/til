# シングルページアプリケーション
単一のWebページでコンテンツ切り替えを行うことで、ページ遷移の必要がなく、ブラウザの挙動に縛られないWeb表現を可能にする
ブラウザ側でできる処理はJavaScriptで終わらせることで、サーバとの通信量を最低限に抑えることが可能
```js
<nav>
  <router-link to="/" active-class="link--active" exact class="link">Home</router-link>
  <router-link to="/user" active-class="link--active" exact class="link">User</router-link>
</nav>
```
`exact`でpathの指定を完全一致にできる
# pathにid付与
```js
export default new Router({
  mode: "history",
  routes: [
    { path: "/", component: Home },
    { path: "/user/:id", component: User }
  ]
});
```
routerはpath指定の時に使う
# routeを使いまわす
`{ path: "/user/:id", component: User, props: true }`
```
export default {
  props: ["id"],
```
propsを使うことで同じ内容を他のページにも表示させることができるようになる
