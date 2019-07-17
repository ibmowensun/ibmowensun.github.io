---
layout: post
title: Difference between HashTabel and HashMap in Java
date: 2007-10-26 13:32:20 +0300
description: Difference between HashTabel and HashMap in Java # Add post description (optional)
img: difference-between-hashmap-hashtable-in-java.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [HashTabel, HashMap]
---
HashTable is thread-synchronized and thread-safe. HashMap is not thread-synchronized, so it is not thread-safe. So in the multi-threaded case to manually synchronize the HashMap the difference is the same as Vector and ArrayList.

### Difference between HashTabel and HashMap in Java

1. HashTable is thread-synchronized and thread-safe. HashMap is not thread-synchronized, so it is not thread-safe. So in the multi-threaded case to manually synchronize the HashMap the difference is the same as Vector and ArrayList.
2. HashTable does not allow null values (both key and value are not allowed), HashMap allows null values (both key and value can be).
3. HashTable has a contains (Object value) function, the same as the containsValue (Object value) function.
4. HashTable uses Enumeration, HashMap uses Iterator.
The above are just the differences in the surface, and their implementation is also very different.
5. The default size of the hash array in HashTable is 11, and the added method is old*2+1. The default size of the hash array in HashMap is 16, and must be an exponent of 2.
6. The use of hash values is different, HashTable directly uses the object's hashCode, the code is like this:

```
int hash = key.hashCode();
　　int index = (hash & 0x7FFFFFFF) % tab.length;
　　而HashMap重新计算hash值，而且用与代替求模：
　　int hash = hash(k);
　　int i = indexFor(hash, table.length);
　　static int hash(Object x) {
　　int h = x.hashCode();
　　h += ~(h << 9);
　　h ^= (h >>> 14);
　　h += (h << 4);
　　h ^= (h >>> 10);
　　return h;
　　}
　　static int indexFor(int h, int length) {
　　return h & (length-1);
　　} 

```


![Quick comparing:](https://www.google.com/url?sa=i&source=imgres&cd=&cad=rja&uact=8&ved=2ahUKEwjarZ6FzLvjAhVKLo8KHTuvAjcQjRx6BAgBEAU&url=https%3A%2F%2Fstackoverflow.com%2Fquestions%2F40471%2Fdifferences-between-hashmap-and-hashtable&psig=AOvVaw0X28KEGnvYzQuxAkpGfUtv&ust=1563440547215549)

