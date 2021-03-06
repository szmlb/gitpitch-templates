## gitpitchテンプレート

---

### Markdownのおさらい

***

- hoge
	- hoge
		- hoge

1. **太字**
2. *イタリック*
3. *** イタリック+太字 ***

@snap[south]
@size[small](https://qiita.com/kamorits/items/6f342da395ad57468ae3)
@snapend

---

### スライドを確認

- https://gitpitch.com/user/repo にアクセスしてスライドを確認できる
- ブランチを指定する場合は https://gitpitch.com/user/repo/branch とする
- １つのリポジトリで複数のスライドを作りたい場合, スライドごとにディレクトリを用意する
- スライドごとに https://gitpitch.com/user/repo/(branch)?p=directory にアクセスすればOK

---

### 文字の色やサイズを調整

- @size[small](小), @size[medium](中),  @size[large](大), @size[x-large](特大), @size[xx-large](超特大), なんもなし
- @size[10px](10px), @size[15px](15px), @size[20px](20px), @size[30px](30px), @size[40px](40px)
- @color[red](赤), @color[blue](青), @color[green](緑), @color[white](白),  @color[black](黒)
- **@color[royalblue](いい感じの青)**,  **@color[midnightblue](深い青)**, **@color[mediumblue](中くらいの青)**, **@color[dodgerblue](よくわからない青)**
- ＠sizeや＠colorは１つの行の中で5個までしか書けないっぽい

@snap[south]
@size[small](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
@size[small](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)
@snapend

---

### 文字を表示する位置を指定

+++?color=white

@snap[north]
North
@snapend

@snap[east]
East
@snapend

@snap[south]
South
@snapend

@snap[west]
West
@snapend

@snap[midpoint]
MidPoint
@snapend

@snap[north-east]
North-East
@snapend

@snap[south-east]
South-East
@snapend

@snap[south-west]
South-West
@snapend

@snap[north-west]
North-West
@snapend

@snap[midpoint]
MidPoint
@snapend

+++?color=white

@snap[north span-100]
### spanの使い方
@snapend

@snap[midpoint span-10]
span-10だとこうなる
@snapend

@snap[west span-30]
span-30だとこうなる
@snapend

@snap[south span-100]
span-100だとこうなる
@snapend

---

### ボックスで囲まれたテキストの挿入

+++?color=white

@snap[north-west span-35]
@box[bg-green text-white demo-box-pad](1. Plan#Lorem ipsum dolor sit amet eiusmod)
@snapend

@snap[north-east span-35]
@box[bg-orange text-white rounded demo-box-pad](2. Build#Sed do eiusmod tempor labore)
@snapend

@snap[south-east span-35]
@box[bg-pink text-white demo-box-pad](3. Measure#Cupidatat non proident sunt in)
@snapend

@snap[south-west span-35]
@box[bg-blue text-white waved demo-box-pad](4. Repeat#Ut enim ad minim veniam prodient)
@snapend

@snap[midpoint span-35]
@box[bg-black text-white demo-box-pad](center)
@snapend

---

### 引用

+++?color=white

@snap[west span-50]
@quote[Hoge piyo fuga]
@snapend

@snap[east span-50]
@quote[Hoge piyo fuga](@szmlb)
@snapend

---

### 順番にアニメーション表示

- Java
- JavaScript |
- Kotlin |
- Go |
- Scala |

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

@title[画像の読み込み]

### 画像の読み込み

![腹たつ](assets/img/Asset.jpg)

+++?image=assets/img/Asset.jpg&position=left&size=50% 50%&color=white

@snap[north]
### 画像と文字の共存 (background)
@snapend

@snap[east span-50]
休んでもいいじゃない, 人間だもの
@snapend

@snap[south]
@size[small](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)
@snapend

+++?color=white

@snap[north]
### 画像と文字の共存 (inline)
@snapend

@snap[west span-50]
![腹たつ](assets/img/Asset.jpg)
@snapend

@snap[east span-50]
休んでもいいじゃない, 人間だもの
@snapend

--- 

### リンクから画像を表示

![Logo](https://onetapbeyond.github.io/resource/img/samba/new-samba-deploy.jpg)


---

### youtubeの動画を表示

![Video](https://www.youtube.com/embed/mkiDkkdGGAQ) 

--- 

### 擬似コード

- やり方がわからない
