# Jekyll

Jekyll은 static site generating software로 마크다운 파일들을 기본으로 해서 웹 페이지를 쉽고 빠르게 제작할 수가 있게 해주는 프로그램이다. Github가 Jekyll 기반으로 운영이 되기 때문에 개인 블로그 운영에 정말 많이 사용되는 프로그램이다. 



## Overall Flow

Jekyll의 전체적인 flow를 설명에 필요한 가장 중요한 파일들은 아래와 같다. 

```
├── _config.yml
├── _includes
├── _layouts
├── _site
└── index.html
```

index.html(또는 index.md) 는 site의 home 역할을 한다. 이후에 permalink등으로 변경할 수 는 있지만 우선 index.html을 home으로 한다고 하자. 

Jekyll이 site를 만드는데 가장 중요한 역할을 하는 것은 **Front Matter(YAML)** 이다. 

```yaml
---
layout: post
title: Blogging Like a Hacker
---
```

Front Matter는 위와 같이 **HTML** 이나 **Markdown** 파일의 상단에 적히는 내용이다. 여기에는 소위 **Variable**이라고 하는 것을 정의해주는데, <span style="color:blue">**layout, permalink, published**</span> 등의 **predefined global variable** 을 포함한 여러 variable들이 존재하고 이를 활용해서 효율적인 디자인을 할 수 있다.

**layout** 은 **_layouts** 에 저장된 html파일을 그대로 불러오는 역할을 한다. 따라서 페이지마다 새로운 layout을 만드는 것이 아니라 기존에 썼던 layout을 불러올 수 있다. 

**title** 등의 variable과 같이 site, page마다 달라지는 변수들은 liquid 문법 형태로 다양하게 활용할 수 있다. liquid 문법으로 **_includes** 에서 미리 만들어둔 페이지의 단위체들을 불러와서 재활용도 가능하다. 

```yaml
---
title: My page
my_variable: footer_company_a.html
---
```

````
{% raw %}{% if page.my_variable %}
{% include {{ page.my_variable }} %}
{% endif %}
<title>{{ page.title }}</title>{% endraw %}
````

>**cf.** Jekyll에서 위와 같이 liquid code를 code block 안에 넣고 싶다면
>
>코드 양 끝에 `{% raw %}{% raw %}{% endraw %}` 와 `{% raw %}{% endraw %}{% endraw %}` 를 붙여주면 된다. 



마지막으로 **config.yml** 에서는 site의 전체적인 information, configuration등을 관리한다. 자세한 정보는 https://jekyllrb.com/docs/configuration/ 에서 확인할 수 있다. 

위와 같은 형태로 HTML과 Markdown파일을 적어주면 최종적으로 Jekyll에서 generate해준 site들은 **_site** 폴더에 들어가게 된다. 

