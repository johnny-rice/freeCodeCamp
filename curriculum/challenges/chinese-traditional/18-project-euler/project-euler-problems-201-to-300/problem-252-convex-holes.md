---
id: 5900f4691000cf542c50ff7b
title: '問題252：凸孔'
challengeType: 1
forumTopicId: 301900
dashedName: problem-252-convex-holes
---

# --description--

Given a set of points on a plane, we define a convex hole to be a convex polygon having as vertices any of the given points and not containing any of the given points in its interior (in addition to the vertices, other given points may lie on the perimeter of the polygon).

作爲示例，下面的圖像示出了一組二十個點和一些這樣的凸孔。 顯示爲紅色七邊形的凸孔具有等於1049694.5平方單位的面積，這是給定點集上的凸孔的最高可能區域。

<img alt="set of twenty points and convex holes on plane" src="https://cdn.freecodecamp.org/curriculum/project-euler/convex-holes.gif" style="background-color: white; padding: 10px; display: block; margin-right: auto; margin-left: auto; margin-bottom: 1.2rem;" />

For our example, we used the first 20 points ($T_{2k − 1}$, $T_{2k}$), for $k = 1, 2, \ldots, 20$, produced with the pseudo-random number generator:

$$\begin{align}   S_0 & = 290\\,797 \\\\
  S_{n+1} & = {S_n}^2 \\; \text{mod} \\; 50\\,515\\,093 \\\\ T_n & = (S_n \\; \text{mod} \\; 2000) − 1000 \end{align}$$

i.e. (527, 144), (−488, 732), (−454, −947), …

What is the maximum area for a convex hole on the set containing the first 500 points in the pseudo-random sequence? Specify your answer including one digit after the decimal point.

# --hints--

`convexHoles()` should return `104924`.

```js
assert.strictEqual(convexHoles(), 104924);
```

# --seed--

## --seed-contents--

```js
function convexHoles() {

  return true;
}

convexHoles();
```

# --solutions--

```js
// solution required
```
