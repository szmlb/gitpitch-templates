# gitpitchテンプレート

---

### ソースコードを表示

```
  defmodule GenMetrics.GenStage.Monitor do
	use GenServer
	alias GenMetrics.GenStage.Manager
	alias GenMetrics.GenStage.Monitor
	alias GenMetrics.GenStage.Pipeline
	alias GenMetrics.GenStage.Window
	alias GenMetrics.Reporter
	alias GenMetrics.Utils.Runtime

	@moduledoc false
	@handle_demand :handle_demand
	@handle_events :handle_events
	@handle_call   :handle_call
	@handle_cast   :handle_cast
	
	defstruct pipeline: %Pipeline{}, metrics: nil, start: 0, duration: 0
```

---

### 指定したコードだけハイライト表示

```
var str1 = 'hello world';
var flag = true;
var result = 10 + 20;


console.log( str1 );
console.log( str2 );
console.log( str3 );
```
@[2](flagに「true」を代入)


---

### 順番にアニメーション表示

- Java
- JavaScript |
- Kotlin |
- Go |
- Scala |

---

### スライドを確認
 
- https://gitpitch.com/user/repo にアクセスしてスライドを確認できる
- ブランチを指定する場合は https://gitpitch.com/user/repo/branch とする
- １つのリポジトリで複数のスライドを作りたい場合, スライドごとにディレクトリを用意する
- スライドごとに https://gitpitch.com/user/repo/(branch)?p=directory にアクセスすればOK

---

### 数式

- [MathJax](http://docs.mathjax.org/en/latest/index.html)を使う
- MathJaxに関しては[この記事](https://qiita.com/PlanetMeron/items/63ac58898541cbe81ada)が参考になる
- 式をこんな感じで ${\bf x}$ 本文の中に埋め込める
- 式ごとに改行して表示
$$ \boldsymbol{\mu} $$
$$ {\bf x} $$
- =で整列して表示
`
\begin{align}
f(x) &= a \\
g(x) &= b
\end{align}
`
