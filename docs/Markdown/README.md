# Markdown

Markdown은 HTML로 변환이 가능한 텍스트 문서이기 때문에 HTML을 그대로 적을 수 있고, CSS등의 활용도 가능하다. 



## Table of Contents ##

> #### for Typora
>
> `[toc]` : creates Table of Contents. 
>
> Automatically extracts headers from the file.  

[toc]

> DocToc
>
> `doctoc README.md --github.com` 을 해주면 
>
> `<!-- START doctoc-->` 과 `<!--END doctor-->` 사이에 
>
> Toc가 만들어진다. (`<--` 는 HTML 주석 )

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Basics](#basics)
  - [Header](#header)
  - [Blockquotes](#blockquotes)
  - [List](#list)
  - [Code](#code)
  - [다양한 텍스트 조작](#%EB%8B%A4%EC%96%91%ED%95%9C-%ED%85%8D%EC%8A%A4%ED%8A%B8-%EC%A1%B0%EC%9E%91)
- [Advanced Functions](#advanced-functions)
  - [Code Blocks](#code-blocks)
  - [Math Blocks](#math-blocks)
  - [Tables](#tables)
  - [Links/Images](#linksimages)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->



## Basics

### Header 

`#` 을 1~6개 까지 사용 가능

1에서 6으로 갈 수록 중요도 &#8595; `#` 과 `##` 는 구분선이 존재

> *<u>Examples</u>*
>
> `# h1`
>
> # h1
>
> `### h3`
>
> ### h3



 ### Blockquotes

`>` 를 앞에 붙이면 하나의 layer가 만들어진다. 

중복해서 붙이면 추가적인 layer가 계속 생성된다. 

enter를 누르면 block에서 빠져나올 수 있다. 

> *<u>Examples</u>*
>
> `> blockquote`
>
> > blockquote



### List

`*` 은 bullet point(unordered list), `1.` 은 ordered list를 만들어낸다. 

enter를 누르면 list에서 빠져나올 수 있다. 

> *<u>Examples</u>*
>
> `* unordered list`
>
> * unordered list
>
> `1. ordered list`
>
> 1. Ordered list



### Code

(`) 를 양 끝에 붙여주면, 그 구문은 HTML로 변환되지 않고 그대로 출력이된다. 

> *<u>Examples</u>*
>
> `printf()` 



### 다양한 텍스트 조작

|     Type      |               Usage               |               Result               |
| :-----------: | :-------------------------------: | :--------------------------------: |
|      URL      |     `https://www.google.com`      |      <https://www.google.com>      |
|   Emphasis    |       `*single asterisks*`        |         *single asterisks*         |
|    Strong     |      `**double asterisks**`       |        **double asterisks**        |
| Strikethrough |        `~~Mistaken text~~`        |         ~~Mistaken text~~          |
|  Underlines   |        `<u>Underline</u>`         |          <u>Underline</u>          |
|     Color     | `<span style="color:red"></span>` | <span style="color:red">red</span> |



## Advanced Functions

### Code Blocks

(``` ) 로 코드를 감싸면 하나의 코드 블럭 안에 들어간다. 

( ``` ) 뒤에 어떤 언어인지를 붙여주면 그 언어의 syntax highlighting을 적용시킨다. 

> *<u>Examples</u>*
>
> ```
> ​```C++
> #include <iostream>
> using namespace std;
> cout<<"Hello World!"<<endl;
> ​```
> ```
>
> ```c++
> #include <iostream>
> using namespace std;
> cout<<"Hello World!"<<endl;
> ```



### Math Blocks

`$$` 로 텍스트를 감싸면 *LaTex*를 인식하는 block을 만들어준다.  

> *<u>Examples</u>*
>
> ```latex
> + - = ! / ( ) [ ] < > | ' : * \times \pm \mp
> ```
>
> $$
> + - = ! / () [] < > | ' : * \times \pm \mp
> $$
>
> ```latex
> \forall x \in X, \quad \exists y \leq \epsilon
> ```
>
> $$
> \forall x \in X, \quad \exists y \leq \epsilon
> $$
>
> ```latex
> \alpha, \beta, \gamma, \Gamma, \pi, \Pi, \phi, \varphi, \mu, \Phi
> ```
>
> $$
> \alpha, \Alpha, \beta, \Beta, \gamma, \Gamma, \pi, \Pi, \phi, \varphi, \mu, \Phi
> $$
>
> ```latex
> \cos (2\theta) = \cos^2 \theta - \sin^2 \theta
> ```
>
> $$
> \cos (2\theta) = \cos^2 \theta - \sin^2 \theta
> $$
>
> ```latex
> \lim\limits_{x \to \infty} \exp(-x) = 0
> ```
>
> $$
> \lim\limits_{x \to \infty} \exp(-x) = 0
> $$
>
> ```latex
> a \bmod b, x \equiv a \pmod{b}
> ```
>
> $$
> a \bmod b, x \equiv a \pmod{b}
> $$
>
> ```latex
> f(n) = n^5 + 4n^2 + 2 |_{n=17}
> ```
>
> $$
> f(n) = n^5 + 4n^2 + 2 |_{n=17}
> $$
>
> ```latex
> \frac{n!}{k!(n-k)!} = \binom{n}{k}, ^3/_7
> ```
>
> $$
> \frac{n!}{k!(n-k)!} = \binom{n}{k}, ^3/_7
> $$
>
> ```latex
> \sqrt{\frac{a}{b}}, \sqrt[n]{1+x+x^2+x^3+\dots+x^n}
> ```
>
> $$
> \sqrt{\frac{a}{b}}, \sqrt[n]{1+x+x^2+x^3+\dots+x^n}
> $$
>
> ```latex
> \sum \prod \int \iint \iiint \idotsint \oint
> ```
>
> $$
> \sum \prod \int \iint \iiint \idotsint \oint
> $$
>
> ```latex
> \sum_{\substack{
>    0<i<m \\
>    0<j<n
>   }} 
>  P(i,j)
> ```
>
> $$
> \sum_{\substack{
>    0<i<m \\
>    0<j<n
>   }} 
>  P(i,j)
> $$
>
> ```latex
> \int\limits_a^b
> ```
>
> $$
> \int\limits_a^b
> $$
>
> ```latex
> ( a ), [ b ], \{ c \}, | d |, \| e \|,
> \langle f \rangle, \lfloor g \rfloor,
> \lceil h \rceil, \ulcorner i \urcorner,
> / j \backslash
> ```
>
> $$
> ( a ), [ b ], \{ c \}, | d |, \| e \|,
> \langle f \rangle, \lfloor g \rfloor,
> \lceil h \rceil, \ulcorner i \urcorner,
> / j \backslash
> $$
>
> ```latex
> A_{m,n} = 
>  \begin{pmatrix}
>   a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
>   a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
>   \vdots  & \vdots  & \ddots & \vdots  \\
>   a_{m,1} & a_{m,2} & \cdots & a_{m,n} 
>  \end{pmatrix}
> ```
>
> $$
> A_{m,n} = 
>  \begin{pmatrix}
>   a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
>   a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
>   \vdots  & \vdots  & \ddots & \vdots  \\
>   a_{m,1} & a_{m,2} & \cdots & a_{m,n} 
>  \end{pmatrix}
> $$
>
> ```latex
> M = \begin{bmatrix}
>        \frac{5}{6} & \frac{1}{6} & 0           \\[0.3em]
>        \frac{5}{6} & 0           & \frac{1}{6} \\[0.3em]
>        0           & \frac{5}{6} & \frac{1}{6}
>      \end{bmatrix}
> ```
>
> $$
> M = \begin{bmatrix}
>        \frac{5}{6} & \frac{1}{6} & 0           \\[0.3em]
>        \frac{5}{6} & 0           & \frac{1}{6} \\[0.3em]
>        0           & \frac{5}{6} & \frac{1}{6}
>      \end{bmatrix}
> $$
>
> ```latex
> 50 \text{ apples} \times 100 \text{ apples}
>  = \text{lots of apples}^2
> ```
>
> $$
> 50 \text{ apples} \times 100 \text{ apples}
>  = \text{lots of apples}^2
> $$
>
> ```latex
> a' a'' \bar{a} \dot{a} \ddot{a} \overrightarrow{AB}\vec{a}
> ```
>
> $$
> a' a'' \bar{a} \dot{a} \ddot{a} \overrightarrow{AB} \vec{a}
> $$
>
> ```latex
> k = {\color{red}x} \mathbin{\color{blue}-} 2
> ```
>
> $$
> k = {\color{red}x} \mathbin{\color{blue}-} 2
> $$
>
> ```latex
> f(n) =
>   \begin{cases}
>     n/2       & \quad \text{if } n \text{ is even}\\
>     -(n+1)/2  & \quad \text{if } n \text{ is odd}
>   \end{cases}
> ```
>
> $$
> f(n) =
>   \begin{cases}
>     n/2       & \quad \text{if } n \text{ is even}\\
>     -(n+1)/2  & \quad \text{if } n \text{ is odd}
>   \end{cases}
> $$
>
> ```latex
> a \quad a \qquad a \, a \: a \; a \! a
> ```
>
> $$
> a \quad a \qquad a \, a \: a \; a \! a
> $$
>
> ```latex
> \therefore \because \uparrow \downarrow \rightarrow \leftarrow
> ```
>
> $$
> \therefore \because \uparrow \downarrow \rightarrow \leftarrow
> $$



### Tables

기본 구조는 아래와 같다. 

```
| Header1 | Header 2 | --> table headers
| ------- | -------- | --> size of cells 
( :----- = left align, ----: = right align, :-----: = center align )
| Content Cell | Cotent Cell |
```



### Links/Images

**internal link**: `[link name](#header name)`

> *<u>Example</u>*
>
> `[example link](#Table of Contents)`
>
> [example link](#Table of Contents)

**external link**: `[link name](site link)`

>*<u>Example</u>*
>
>`[Google](https://www.google.com)`
>
>[Google](https://www.google.com)

**images**: `![image name](path/url to image)` 









