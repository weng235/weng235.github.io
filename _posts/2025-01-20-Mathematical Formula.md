---
title: 高等数学常用公式
description: 渐近线、微分方程、等价无穷小、麦克劳林展开的公式大全
date: 2025-01-20 8:00:00 +0800
categories: [数学]
tags: [math]
math: true
---

## 渐近线

1. **水平渐近线**  
   当 $$ x \to +\infty $$ 或 $$ x \to -\infty $$ 时，$$ y \to c $$，其中 $$ y = c $$ 就是 $$ f(x) $$ 的水平渐近线。

2. **铅直渐近线**  
   当 $$ x \to a $$ 时，$$ y \to +\infty $$ 或 $$ y \to -\infty $$，其中 $$ x = a $$ 就是 $$ f(x) $$ 的铅直渐近线。

3. **斜渐近线**  
   当 $$ x \to \infty $$ 时，$$ \frac{y}{x} $$ 的极限为某一常数 $$ k $$，则 $$ y = kx + b $$ 为斜渐近线。

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

1. **指数函数**：
$$
e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots
$$

2. **正弦函数**：
$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots
$$

3. **余弦函数**：
$$
\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots
$$

4. **自然对数**：
$$
\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \cdots \quad (|x| < 1)
$$

5. **反正切函数**：
$$
\tan^{-1} x = x - \frac{x^3}{3} + \frac{x^5}{5} - \frac{x^7}{7} + \cdots \quad (|x| \leq 1)
$$

6. **平方根函数**：
$$
\sqrt{1+x} = 1 + \frac{x}{2} - \frac{x^2}{8} + \frac{x^3}{16} - \cdots \quad (|x| < 1)
$$

7. **几何级数**：
$$
\frac{1}{1-x} = 1 + x + x^2 + x^3 + \cdots \quad (|x| < 1)
$$
