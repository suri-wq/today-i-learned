# flex property

A shorthand for setting flex-grow, flex-shrink, flex-basis of a flex item.

### Syntax

```css
 flex: [flex-grow] [flex-shrink] [flex-basis];
```

### Default

```css
 flex: 0 1 auto;
```

### Parameters
#### 1. flex-grow(number)

1. Defines the ability for a flex item to grow if there is space available.

2. Default is 0 (it will not grow).

3. A value of 1 means it can grow to fill the space proportionally.



#### 2. flex-shrink (number):

1. Defines the ability for a flex item to shrink if there is not enough space.

2. Default is 1 (it will shrink if necessary).

3. A value of 0 means it will not shrink even if the container is smaller.



#### 3. flex-basis (length | auto):

1. Defines the default size of an element before the remaining space is distributed.

2. It can be a specific size (e.g., 200px) or auto, which means it is based on its content.
