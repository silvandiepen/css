---
title: Viewport
---

# Understanding CSS Viewport Units: A Comprehensive Guide with Examples

Viewport units in CSS provide a powerful way to create responsive designs that adapt seamlessly to various screen sizes and orientations. These units allow developers to specify lengths and sizes relative to the viewport's dimensions, ensuring consistent layout regardless of the device being used. In this guide, we'll explore all viewport units, including the latest modifiers for small, large, and dynamic viewport sizes, along with practical examples.

## 1. Viewport Width (vw) and Viewport Height (vh)

Viewport width (vw) and viewport height (vh) are perhaps the most commonly used viewport units. They represent 1% of the viewport's width and height, respectively.

**Example:**
```css
.container {
  width: 50vw; /* 50% of viewport width */
  height: 80vh; /* 80% of viewport height */
  background-color: lightblue;
}
```
## 2. Viewport Minimum (vmin) and Viewport Maximum (vmax)

Viewport minimum (vmin) and viewport maximum (vmax) units are useful for scenarios where you want elements to scale relative to the smaller or larger dimension of the viewport.

**Example:**
```css
.container {
  width: 50vmin; /* 50% of the smaller dimension (width or height) */
  height: 70vmax; /* 70% of the larger dimension (width or height) */
  background-color: lightgreen;
}
```

## 3. Small Viewport Units (sv-)

Small viewport units, denoted by the prefix "sv-", adjust their size based on the viewport size while considering active UA UI elements.

**Example:**
```css
.container {
  height: 100svh; /* 100% of available viewport height excluding active UI */
  width: 100svw; /* 100% of available viewport width excluding active UI */
  background-color: lightcoral;
}
```

## 4. Large Viewport Units (lv-)

Large viewport units, marked by the prefix "lv-", calculate their size without considering UA UI elements, functioning similarly to the top-level units.

**Example:**

```css
.container {
  height: 90lvh; /* 90% of viewport height ignoring UI */
  width: 80lvw; /* 80% of viewport width ignoring UI */
  background-color: lightyellow;
}
```

## 5. Dynamic Viewport Units (dv-)

Dynamic viewport units, prefixed with "dv-", adjust automatically when UA UI elements expand or retract, providing flexibility in responsive designs.

**Example:**
```css
.container {
  height: 100dvh; /* Automatically adjusts to available screen height */
  width: 100dvw; /* Automatically adjusts to available screen width */
  background-color: lightsalmon;
}
```

## 6. Viewport Width Inline (vi) and Viewport Width Block (vb)

Viewport width inline (vi) and viewport width block (vb) units are relative to the size of the initial containing block. Vi is relative to the inline size (width) of the initial containing block, while vb is relative to the block size (height) of the initial containing block.

**Example:**
```css
.container {
  width: 50vi; /* 50% of the inline size of the initial containing block */
  height: 60vb; /* 60% of the block size of the initial containing block */
  background-color: lightpink;
}
```
