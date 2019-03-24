# java复习笔记

## map 的使用 <https://docs.oracle.com/javase/8/docs/api/index.html>

1. 初始化：

   ``` java
   Map<String, String> map = new HashMap<String, String>();
   ```

2. 插入元素：

   ```java
   map.put("key1", "value1");
   ```

3. 获取元素：

   ```java
   map.get("key1")
   ```

4. 移除元素：

   ```java
   map.remove("key1");
   ```

5. 清空:

   ```java
   map.clear();
   ```

   ### 常用API

   | clear()                       | 从 Map 中删除所有映射                                        |
   | ----------------------------- | ------------------------------------------------------------ |
   | remove(Object key)            | 从 Map 中删除键和关联的值                                    |
   | put(Object key, Object value) | 将指定值与指定键相关联                                       |
   | putAll(Map t)                 | 将指定 Map 中的所有映射复制到此 map                          |
   | entrySet()                    | 返回 Map 中所包含映射的 Set 视图。Set 中的每个元素都是一个 Map.Entry 对象，可以使用 getKey() 和 getValue() 方法（还有一个 setValue() 方法）访问后者的键元素和值元素 |
   | keySet()                      | 返回 Map 中所包含键的 Set 视图。删除 Set 中的元素还将删除 Map 中相应的映射（键和值） |
   | values()                      | 返回 map 中所包含值的 Collection 视图。删除 Collection 中的元素还将删除 Map 中相应的映射（键和值） |
   | get(Object key)               | 返回与指定键关联的值                                         |
   | containsKey(Object key)       | 如果 Map 包含指定键的映射，则返回 true                       |
   | containsValue(Object value)   | 如果此 Map 将一个或多个键映射到指定值，则返回 true           |
   | isEmpty()                     | 如果 Map 不包含键-值映射，则返回 true                        |
   | size()                        | 返回 Map 中的键-值映射的数目                                 |