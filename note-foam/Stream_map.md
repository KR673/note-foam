[toc]

## toMap

```javascript
list = [{
    name: "小明",
    age: 12
}, {
    name: "小红",
    age: 13
}]

// 转化为--> key = name, value = age 的map
map = {
    "小明": 12,
    "小红": 13
}
```

```java
list.stream()
    .collect(Collectors
        .toMap(t -> t.getName(), t -> t.getAge(), (v1, v2) -> v1);
```