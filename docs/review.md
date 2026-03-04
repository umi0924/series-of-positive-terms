# 正项级数判别法要点复习

本页汇总了判断正项级数 $\sum_{n=1}^{\infty} a_n$ ($a_n > 0$) 敛散性的基本判别法。

---

### 1. 必要条件 (第 n 项发散判别法)
若 $\lim_{n \to \infty} a_n \neq 0$ 或极限不存在，则级数 $\sum a_n$ 发散。

### 2. 比值判别法 (Ratio Test / D'Alembert Test)
设 $\rho = \lim_{n \to \infty} \frac{a_{n+1}}{a_n}$：
* 若 $\rho < 1$，级数收敛；
* 若 $\rho > 1$ 或 $\rho = \infty$，级数发散；
* 若 $\rho = 1$，判别法失效。

### 3. 根值判别法 (Root Test / Cauchy Test)
设 $\rho = \lim_{n \to \infty} \sqrt[n]{a_n}$：
* 若 $\rho < 1$，级数收敛；
* 若 $\rho > 1$ 或 $\rho = \infty$，级数发散；
* 若 $\rho = 1$，判别法失效。

### 4. 极限比较判别法 (Limit Comparison Test)
设 $b_n$ 为参考级数，且 $L = \lim_{n \to \infty} \frac{a_n}{b_n}$：
* 若 $0 < L < \infty$，则 $\sum a_n$ 与 $\sum b_n$ 同敛散；
* 若 $L = 0$ 且 $\sum b_n$ 收敛，则 $\sum a_n$ 收敛；
* 若 $L = \infty$ 且 $\sum b_n$ 发散，则 $\sum a_n$ 发散。

### 5. 直接比较判别法 (Direct Comparison Test)
设对所有 $n \ge N$，均有 $0 \le a_n \le b_n$：
* 若 $\sum b_n$ 收敛，则 $\sum a_n$ 收敛；
* 若 $\sum a_n$ 发散，则 $\sum b_n$ 发散。

### 6. 积分判别法 (Integral Test)
设 $f(x)$ 是定义在 $[1, \infty)$ 上的连续、非负、递减函数，且 $f(n) = a_n$：
* 级数 $\sum_{n=1}^{\infty} a_n$ 与反常积分 $\int_{1}^{\infty} f(x) dx$ 同敛散。

---

### 附：常用参考级数
* **p-级数**：$\sum_{n=1}^{\infty} \frac{1}{n^p}$ 在 $p > 1$ 时收敛，$p \le 1$ 时发散。
* **几何级数**：$\sum_{n=0}^{\infty} ar^n$ ($a \neq 0$) 在 $|r| < 1$ 时收敛，$|r| \ge 1$ 时发散。