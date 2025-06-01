# grid-template

A shorthand property for defining structure of rows and columns in a grid layout.

### Syntax

```css
 flex: [flex-grow] [flex-shrink] [flex-basis];
```

### Default

```css
.dice-container {
    display: grid;
    grid-template: auto auto / repeat(5, 1fr);
    gap: 20px;
}
```

This is shorthand for:
```css
    grid-template-rows: auto auto;
    grid-template-columns: repeat(5, 1fr);
```

**`auto auto` — Rows**  
This means there are **2 rows**, and each row’s height is determined **automatically** based on its content.

**`repeat(5, 1fr)` — Columns**  
`repeat(5, 1fr)` creates **5 equal-width columns**.  
`1fr` means “one fraction” of the available space.  
So you're building a **5-column layout**, and each column takes up an **equal portion** of the row width.

**`gap: 20px;`**  
This adds **20px of space** between rows and columns — a **uniform spacing grid**.
