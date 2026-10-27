# Task 10: CSS - Laundry Services Hero Image Animation

Animated hero image for the laundry services page, built with plain HTML and CSS (no JavaScript).

## Files

- `index.html` - page structure (navbar + hero section)
- `style.css` - styling, media queries, hover effect and the animation, linked from the HTML
- `laundry.png` - laundry illustration that is animated
- `Readme.md` - this file

## Animation

```css
.hero-right img {
    animation: orbit 6s linear infinite;
}

@keyframes orbit {
    0%   { transform: rotate(0deg)   translateX(25px) rotate(0deg)    scale(1, 1); }
    25%  { transform: rotate(90deg)  translateX(25px) rotate(-90deg)  scale(0.9, 1.08); }
    50%  { transform: rotate(180deg) translateX(25px) rotate(-180deg) scale(1.06, 0.92); }
    75%  { transform: rotate(270deg) translateX(25px) rotate(-270deg) scale(0.9, 1.08); }
    100% { transform: rotate(360deg) translateX(25px) rotate(-360deg) scale(1, 1); }
}
```

- **Orbit rotation:** `rotate()` followed by `translateX()` moves the image around a circle. The second `rotate()` with the opposite angle keeps the image upright while it travels.
- **Squeeze:** `scale()` values change at 25%, 50% and 75% so the image is squeezed (narrower and taller, then wider and shorter) at certain points of the orbit.
- **Loop:** `6s linear infinite` makes it run smoothly and forever.

The button hover effect, responsive layout and mobile hamburger menu from the earlier tasks still work.

## How to run

Keep `index.html`, `style.css` and `laundry.png` in the same folder and open `index.html` in a browser.
