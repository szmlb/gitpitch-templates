# slide title

---

### source code

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

### Check the generated slides
 
- Access to the https://gitpitch.com/user/repo 
- or https://gitpitch.com/user/repo/branch, if branch is specified
- If you want to use multiple slides in one repo, make a directory for each slides
- Then, access to https://gitpitch.com/user/repo/(branch)?p=directory

---

### Equation

-`\[
\left( \sum_{k=1}^n a_k b_k \right)^{\!\!2} \leq
 \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
\]`
- \boldsymbol{x}
