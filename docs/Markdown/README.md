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

<!-- END doctoc generated TOC please keep comment here to allow auto update -->



## Basics

### Header 

`#` 을 1~6개 까지 사용 가능

1에서 6으로 갈 수록 중요도 &#8595; `#` 과 `##` 는 구분선이 존재

> *<u>Example</u>*
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

> *<u>Example</u>*
>
> `> blockquote`
>
> > blockquote

### List

`*` 은 bullet point(unordered list), `1.` 은 ordered list를 만들어낸다. 

enter를 누르면 list에서 빠져나올 수 있다. 

> *<u>Example</u>*
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

> *<u>Example</u>*
>
> `printf()` 

### 다양한 텍스트 조작

|     Type      |               Usage               |               Result               |
| :-----------: | :-------------------------------: | :--------------------------------: |
|      URL      |         `www.google.com`          |      <https://www.google.com>      |
|   Emphasis    |       `*single asterisks*`        |         *single asterisks*         |
|    Strong     |      `**double asterisks**`       |        **double asterisks**        |
| Strikethrough |        `~~Mistaken text~~`        |         ~~Mistaken text~~          |
|  Underlines   |        `<u>Underline</u>`         |          <u>Underline</u>          |
|     Color     | `<span style="color:red"></span>` | <span style="color:red">red</span> |









