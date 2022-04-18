---
marp: true
theme: default+
paginate: true
header: 'Header'
footer: 'Footer'
headingDivider: 2
math: katex
style: @import url('https://unpkg.com/tailwindcss@^2/dist/utilities.min.css');
---

<!-- _class: lead -->
# Sample slide deck

Sample slide deck converted from MarkDown by Marp Next.

@ttyskg

## List structures

### List

* List
* List
  * Sublist
  * Sublist

### Number List

1. first  
1.1. numeric sublist 1-1  
1.2. numeric sublist 1-2
2. second
3. third  
3.1. numeric sublist 3-1  
3.2. numeric sublist 3-2

## Table

|      | col1 | col2 | col3 |
| ---- | ---- | ---- | ---- |
| row1 | item | item | item |
| row2 | item | item | item |
| row3 | item | item | item |

## Figure insert

This is my icon.

![height:250px](./img/icon.png)

Cute owl!

## Code block

FizzBuzz by Python.

```python
def FizzBuzz(n):
    for i in range(n):
        num = i + 1
        if (num % 15) == 0:
            print('FizzBuzz')
        elif (num % 5) == 0:
            print('Buzz')
        elif (num % 3) == 0:
            print('Fizz')
        else:
            print(num)
```

## Math block

Marp Next support KaTex format to write Math equations.

$$
\frac{\partial \theta}{\partial t}= \frac{\partial}{\partial z}
\left[ K(\theta) \left (\frac{\partial \psi}{\partial z} + 1 \right) \right]
$$

## Quote

> Tradition is not the worship of ashes,
> but the preservation of fire.
>
> **Gustav Mahler (Composer)**

## SVG with hyperlinks

<object type="image/svg+xml" data="img/icon.drawio.svg"> </object>

* You can insert a SVG file with clickable hyperlink
  * `<object type="image/svg+xml" data="img/icon.drawio.svg"></object>`
* To enable this function, you should enable `html` option of MARP

## How to use multi-columns mode

In this **default+** theme, a CSS classes, `two-columns`,
is defined for splitting one slide into two columns.  
You can customize the number of columns, width, etc. by slightly changing the CSS class.

<div class='two-columns'>
  <div>

`two-columns` CSS class  

```css
.two-columns {
    display: grid;
    grid-template-columns: 50% 50%;
    padding-bottom: 10px;
}
```

  </div>
  <div>

Markdown/HTML code for using `two-columns`.

```html
<div class='two-columns'>
    <div>

Left pane contents

    </div>
    <div>
        
Right pane

    </div>
</div>

This area is outside the split panes.
```

  </div>
</div>

**Note:** Marp does not render HTML tags by default.
Turn on `Markdown > Marp: Enable HTML` from VS Code setting
([See here](https://github.com/marp-team/marp/discussions/192#discussioncomment-1517399)).

## Two-panes appearance


<div class='two-columns'>
  <div>

### Left pane

**List:**

* List
* List

**Table:**

| col1         | col2       | col3        |
| :----------: | :--------- | ----------: |
| center-align | left-align | right-align |
| item1        | item1      | item3       |

  </div>
  <div>

### Right pane

**Image:**

![height:150px](./img/icon.png)

**Math equation:**

$$
\frac{\partial \theta}{\partial t}= \frac{\partial}{\partial z}
\left[ K(\theta) \left (\frac{\partial \psi}{\partial z} + 1 \right) \right]
$$

  </div>
</div>

This area is outside the split pane.

## Multi-columns

For simple equal-width columns, you can also use the
[Tailwind CSS](https://tailwindcss.com/) utility
([Discussion #192 · marp-team/marp](https://github.com/marp-team/marp/discussions/192)).

```HTML
---
marp: true
style: @import url('https://unpkg.com/tailwindcss@^2/dist/utilities.min.css');
---

# Multi columns in Marp slide

<div class="grid grid-cols-2 gap-2">
<div>

Column 1

</div>
<div>

Column 2

</div>
</div>
```

<div class='grid grid-cols-4 gap-2'>
  <div>

**column 1:**  

* List
  * Sublist
* List

  </div>
  <div>

**column 2:**  
The quick brown fox jumps over the lazy dog.

  </div>
  <div>

**column 3:**  

$$
\frac{\partial \theta}{\partial t}= \frac{\partial}{\partial z}
\left[ K(\theta) \left (\frac{\partial \psi}{\partial z} + 1 \right) \right]
$$

  </div>
  <div>

**column 4:**  

![height:150px](./img/icon.png)

  </div>
</div>
