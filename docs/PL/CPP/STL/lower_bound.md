## std::lower_bound

```c++
template <class ForwardIterator, class T>
ForwardIterator lower_bound (ForwardIterator first, ForwardIterator last, const T& val);
                               
template <class ForwardIterator, class T, class Compare>
ForwardIterator lower_bound (ForwardIterator first, ForwardIterator last, const T& val, Compare comp);       
```

Returns an iterator pointing to the first element in the range `[first,last)` which does not compare less than val.

val 이상의 수 중 가장 앞에 있는 element의 iterator를 return -> 이분탐색