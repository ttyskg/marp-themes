---
marp: true
theme: uranus
paginate: true
header: 'Header'
footer: 'Footer'
headingDivider: 2
math: katex
---

<!-- _class: lead -->
# Sample slide deck

Sample slide deck converted from MarkDown by Marp Next.

@ttyskg

## List structures

test text text

* List
* List
* List
  * Sublist
  * Sublist

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
