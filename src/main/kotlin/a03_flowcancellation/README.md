# Flow cancellation

- Flow のキャンセル方法は、特別なインタフェースが用意されているわけではない
- Flow では通常の Coroutine をキャンセルする方法と同じ方法でキャンセルを行う
- Coroutine では withTimeoutOrNull を利用して、一定時間経過したあとに完了していないければキャンセルができる
  これを利用して Flow をキャンセルしてみると、250msec 分の処理をして、それ以降はキャンセルされ実行されないのが確認できる。
  
  