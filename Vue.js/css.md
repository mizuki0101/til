# cssトランジション
```js
fade-enter {
  opacity: 0;
}
.fade-enter-active {
  transition: opacity 0.5s;
}
.fade-enter-to {
  opacity: 1;
}
.fade-leave {
  opacity: 1;
}
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-leave-to {
  opacity: 0;
}
```

# cssアニメーション
```js
.slide-enter-active {
  animation: slide-in 0.5s;
}

.slide-leave-active {
  animation: slide-in 0.5s reverse;
}

@keyframes slide-in {
  from {
    transform: translateX(100px);
  }
  to {
    transform: translateX(0);
  }
}
```
## トランジションとアニメーションを両方使う
```js
.slide-enter,
.slide-leave-to {
  opacity: 0;
}
.slide-enter-active {
  animation: slide-in 0.5s;
  transition: opacity 1s;
}
```
# animeitonCssを使う
```js
<transition enter-active-class="animated bounce" leave-active-class="animated shake" appear>
```
