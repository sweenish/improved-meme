# improved-meme
A small showcase of a way to manage documentation simply, with releases

## Like math!

The current rendering engine for math is [MathJax](https://www.mathjax.org), but the beta github.dev editor uses [KaTeX](https://katex.org). Both engines are using $\LaTeX$, of which there are many online references.

`$$\lim\limits_{x\to0} \dfrac{1}{1-x}$$` turns into:  
$$\lim\limits_{x\to0} \dfrac{1}{1-x}$$

## Tables!

Plaintext alignment of the pipes (`|`) is not necessary, but it helps the plaintext look nice.

| Column 1 | Column 2      | Result |
-----------|---------------|---------
| A value  | Another value | Result |
| Another row | What. Is. This?! | Result |

## Diagrams

Diagrams can be created using [Mermaid](https://mermaid.js.org/) code blocks. It is worth noting that the diagrams are
not rendered in the beta editor. 

```mermaid
---
title: Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
```

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
