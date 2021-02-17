# std::map

## Functions

### find

*<u>Return value:</u>*

<span style="color:darkblue;">**If found**</span> - Iterator to the element

<span style="color:darkblue;">**Else**</span> - map::end

*<u>Complexity:</u>*

$O(\log{n})$

### insert

*<u>Example:</u>*

```c++
std::map<char,int> mymap;
mymap.insert ( std::pair<char,int>('a',100) );
```

