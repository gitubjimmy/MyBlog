# Variables

## Predefined Variables

YAML 언어에서 사용되는 variable들의 종류와 각 variable들이 가리키는 정보의 실제 위치에 대한 표이다. 

| Type      | Location                             |
| --------- | ------------------------------------ |
| site      | _config.yml                          |
| site.data | yml files in **_data** folder        |
| page      | 해당하는 페이지를 나타내는 html 파일 |

### page

| Variable | Description                              |
| -------- | ---------------------------------------- |
| page.dir | root directory 부터 현재 page까지의 path |



## Defining Variables(YAML)

- YAML is **space sensitive**, each level requires two spaces
- `{% raw %}{% assign profile = site.theme_settings %}{% endraw %}` 페이지 내에서 variable의 이름을 위와 같이 재정의 할 수 있다.
- https://idratherbewriting.com/documentation-theme-jekyll/mydoc_yaml_tutorial

### Simple Mapping

```yaml
"2015":
  Return:
    ReturnHeader:
      ReturnTypeCd: "Et hop !"
```

위와 같은 형태로 `_data/grants.yml` 에 저장되어 있었다면

`{% raw %}{{ site.data.grants.2015.Return.ReturnHeader.ReturnTypeCd }}{% endraw %}` 가 가능하다. 

### list

**YAML**:

```yaml
bikes:
  - title: mountain bikes
  - title: road bikes
  - title: hybrid bikes
```

**Markdown + Liquid:**

```
{% raw %}<ul>
{% for item in site.data.samplelist.bikes %}
<li>{{item.title}}</li>
{% endfor %}
</ul>{% endraw %}
```

**Result:**

>- mountain bikes
>- road bikes
>- hybrid bikes

