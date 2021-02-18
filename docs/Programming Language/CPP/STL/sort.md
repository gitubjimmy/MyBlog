# std::sort

`<algorithm>`에 포함된 함수

*<u>Example:</u>*

**내림차순**

```C++
 sort(arr, arr + 5, greater<int>());
```

**Custom class**

1. 연산자 오버로딩

```c++
bool operator <(const Person &a, const Person &b){
    return a.age < b.age;
}

int main(){
	vector<Person> v;
	sort(v.begin(), v.end());
}
```

2. 사용자 함수 정의

```c++
bool cmp(const Person &a, const Person &b){
    return a.name > b.name;
}

int main(){
	vector<Person> v;
	sort(v.begin(), v.end());
}
```

