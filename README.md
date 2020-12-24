# rfc-css-transform-scale-fixed
A proposal for CSS `transform` `scale` to fixed size.

In CSS we can use `transform` to take advantage of GPU-accelerated animations for elements.

The `scale` functions (`scaleX`, `scaleY`, `scaleZ`, and `scale3d`) let us change the size of an element,
but only allow multipliers on current size.

But we often want to target a specific size, regardless of current size, especially for layout animations.

Proposing new support for scaling to fixed unit sizes.

For example, to scale an element to exactly 10 pixels wide and 20 pixels high:

```css
transform: scale(10px, 20px);
```
