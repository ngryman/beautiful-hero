<div align=center>
  <img width=0 height=500 src="../empty.gif">
  <sup>![](../beautiful-heroes.png)</sub>
  <sup><sup><img width=100% height=0 src="../empty.gif"><img width=0 height=200 src="../empty.gif"></sub></sub>

---

## Code

```markdown
<div align=center>
  <img width=0 height=500 src="../empty.gif">
  <sup>![](../beautiful-heroes.png)
  <sup><sup><img width=100% height=0 src="../empty.gif"><img width=0 height=200 src="../empty.gif">
```

## Explanation

The only possible way to align something vertically is to use tables. But unfortunately they come with a border that we can't remove. I've tried :disappointed:.

There is no hope to find some `vertical-align: middle` element, everything is set `baseline`. So the only way to play with layout is via 3 tags:
 - `img`: it can be freely sized with `width` and `height` attributes. So we can basically create *empty* areas with them.
 - `sup`: it shifts content up, we can use it to compensate space created between images by the generated markup.
 - `sub`: it shifts content down, same thing.
