---
title: 高等数学常用公式
description: 积分的旋转体公式、渐近线、微分方程、等价无穷小、麦克劳林展开的公式大全
date: 2025-01-20 8:00:00 +0800
categories: [数学]
tags: [math]
math: true
---

## 积分的旋转体公式

### 1. 圆盘法（Disk Method）
适用于绕坐标轴旋转的函数。

1. **绕x轴旋转**
   
   $$ V = \pi \int_{a}^{b} [f(x)]^2 dx $$

   其中：
   - $$ f(x) $$ 是曲线的函数
   - $$ x $$ 在区间 $$ [a,b] $$ 上
   - 体积是无穷多个薄圆盘的体积之和

2. **绕y轴旋转**
   
   $$ V = \pi \int_{c}^{d} [g(y)]^2 dy $$

   其中：
   - $$ g(y) $$ 是曲线的反函数 $$ x = g(y) $$
   - $$ y $$ 在区间 $$ [c,d] $$ 上

### 2. 圆环法（Washer Method）
适用于由两个函数围成的区域旋转。

$$ V = \pi \int_{a}^{b} \left( [R(x)]^2 - [r(x)]^2 \right) dx $$

其中：
- $$ R(x) $$ 是外层曲线的半径
- $$ r(x) $$ 是内层曲线的半径
- 体积是无穷多个圆环的体积之和

### 3. 柱壳法（Shell Method）
适用于区域绕y轴旋转，或圆盘法积分较难计算的情况。

1. **绕y轴旋转**
   
   $$ V = 2\pi \int_{a}^{b} x f(x) dx $$

   其中：
   - $$ x $$ 是柱壳的半径
   - $$ f(x) $$ 是柱壳的高度
   - 体积是无穷多个圆柱壳的体积之和

2. **绕x轴旋转**
   
   $$ V = 2\pi \int_{c}^{d} y g(y) dy $$

   其中：
   - $$ y $$ 是柱壳的半径
   - $$ g(y) $$ 是柱壳的高度


---

## 微分方程

### 一阶微分方程

**形式**：
$$ 
\frac{dy}{dx} + P(x)y = Q(x) 
$$

**通解**：
$$ 
y = e^{-\int P(x) \, dx} \left( \int Q(x)e^{\int P(x) \, dx} \, dx + C \right) 
$$

### 二阶微分方程

**形式**：
$$ 
\frac{d^2y}{dx^2} + P(x)\frac{dy}{dx} + Q(x)y = f(x) 
$$

#### 通解

1. **不同实根**：
$$ 
y_c = C_1 e^{r_1x} + C_2 e^{r_2x} 
$$

2. **单一重根**：
$$ 
y_c = (C_1 + C_2x)e^{r_1x} 
$$

3. **共轭复根**：
$$ 
y_c = e^{\alpha x} \left( C_1 \cos(\beta x) + C_2 \sin(\beta x) \right) 
$$

#### 特解

设 $ f(x) = e^{\lambda x} P_m(x) $ 

1. **无根**：
$$ 
y^* = e^{\lambda x} Q_m(x) 
$$

2. **单根**：
$$ 
y^* = x e^{\lambda x} Q_m(x) 
$$

3. **重根**：
$$ 
y^* = x^2 e^{\lambda x} Q_m(x) 
$$

## 常用等价无穷小公式

**基本等价无穷小**:

1.$$ \sin x \sim x $$

2.$$ \tan x \sim x $$

3.$$ e^x - 1 \sim x $$

4.$$ \ln(1+x) \sim x $$

5.$$ \sin x \sim x - \frac{x^3}{6} $$

6.$$ \tan x \sim x + \frac{x^3}{3} $$

7.$$ e^x - 1 \sim x + \frac{x^2}{2} + \frac{x^3}{6} $$

8.$$ \sqrt{1+x} - 1 \sim \frac{x}{2} $$

9.$$ \frac{1}{1+x} \sim 1 - x $$

---

## 常用麦克劳林展开公式
> $$ f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3 + ... + \frac{f^{(n)}(0)}{n!}x^n + R_n(x) $$
{: .prompt-tip }

1. **几何级数**：
$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n \quad (|x| < 1)
$$


2. **指数函数**：
$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}
$$

3. **正弦函数**：
$$
\sin x = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!}
$$

4. **余弦函数**：
$$
\cos x = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{(2n)!}
$$

5. **自然对数**：
$$
\ln(1+x) = \sum_{n=1}^{\infty} \frac{(-1)^{n+1}x^n}{n} \quad (|x| < 1)
$$

6. **反正切函数**：
$$
\tan^{-1} x = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{2n+1} \quad (|x| \leq 1)
$$


