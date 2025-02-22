# Hashing 
## API
!!! Note
    Here, I have listed some commonly used methods. For the complete methods, please refer to [Javadocs](https://docs.oracle.com/javase/8/docs/api/)
### Class `HashSet<E>`
#### Constructors
- `HashSet()`
- `HashSet(Collection<? extends E> c)`: Constructs a new set containing the elements in the specified collection. 
- `HashSet(int initialCapacity)`: Constructs a new, empty set; the backing HashMap instance has the specified initial capacity and default load factor (0.75).
- `HashSet(int initialCapacity, float loadFactor)`: Constructs a new, empty set; the backing HashMap instance has the specified initial capacity and the specified load factor.
#### Method
- `boolean add(E e)`: Adds the specified element to this set if it is not already present.
- `void clear()`: Removes all of the elements from this set.
- `boolean contains(Object o)`: Returns true if this set contains the specified element.
- `boolean isEmpty()`: Returns true if this set contains no elements.
- `boolean remove(Object o)`: Removes the specified element from this set if it is present.
- `int size()`: Returns the number of elements in this set (its cardinality).
- `Object clone()`: Returns a shallow copy of this HashSet instance: the elements themselves are not cloned.

### Class `HashMap<K,V>`
#### Constructors
- `HashMap()`
- `HashMap(Map<? extends K,? extends V> m)`: Constructs a new HashMap with the same mappings as the specified Map.
- `HashMap(int initialCapacity)`: Constructs an empty HashMap with the specified initial capacity and the default load factor (0.75).
- `HashMap(int initialCapacity, float loadFactor)`: Constructs an empty HashMap with the specified initial capacity and load factor.
#### Method
- `void clear()`: Removes all of the mappings from this map.
- `Object clone()`: Returns a shallow copy of this HashMap instance: the keys and values themselves are not cloned.
- `boolean containsKey(Object key)`: Returns true if this map contains a mapping for the specified key.
- `boolean containsValue(Object value)`: Returns true if this map maps one or more keys to the specified value.
- `V get(Object key)`: Returns the value to which the specified key is mapped, or null if this map contains no mapping for the key.
- `Set<Map.Entry<K,V>> entrySet()`: Returns a Set view of the mappings contained in this map.
- `void forEach(BiConsumer<? super K,? super V> action)`: Performs the given action for each entry in this map until all entries have been processed or the action throws an exception.
- `V getOrDefault(Object key, V defaultValue)`: Returns the value to which the specified key is mapped, or defaultValue if this map contains no mapping for the key.
- `boolean isEmpty()`: Returns true if this map contains no key-value mappings.
- `int size()`: Returns the number of key-value mappings in this map.
- `Set<K> keySet()`: Returns a Set view of the **keys** contained in this map.
- `Collection<V> values()`: Returns a Collection view of the **values** contained in this map.
- `V put(K key, V value)`
Associates the specified value with the specified key in this map.
- `void putAll(Map<? extends K,? extends V> m)`: Copies all of the mappings from the specified map to this map.
- `V putIfAbsent(K key, V value)`: If the specified key is not already associated with a value (or is mapped to null) associates it with the given value and returns null, else returns the current value.
- `V remove(Object key)`: Removes the mapping for the specified key from this map if present.
- `boolean remove(Object key, Object value)`: Removes the entry for the specified key only if it is currently mapped to the specified value.
- `V replace(K key, V value)`: Replaces the entry for the specified key only if it is currently mapped to some value.
- `boolean replace(K key, V oldValue, V newValue)`: Replaces the entry for the specified key only if currently mapped to the specified value.


## Reference
- [Javadocs/HashSet](https://docs.oracle.com/javase/8/docs/api/java/util/HashSet.html)
- [Javadocs/HashMap](https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html)