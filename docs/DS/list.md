# List
## API
!!! Note
    Here, I have listed some commonly used methods. For the complete methods, please refer to [Javadocs](https://docs.oracle.com/javase/8/docs/api/)
### Class `ArrayList<E>`
!!! Warning
    ArrayList is not array! (`ArrayList<E> <: List<E>`)
#### Constructors
- `ArrayList()`: Constructs an empty list with an initial capacity of ten.
- `ArrayList(Collection<? extends E> c)`: Constructs a list containing the elements of the specified collection, in the order they are returned by the collection's iterator.
- `ArrayList(int initialCapacity)`: Constructs an empty list with the specified initial capacity.
#### Method
- `void clear()`: Removes all of the elements from this list.
- `boolean isEmpty()`
- `boolean contains(Object o)`
- `E get(int index)`
- `int size()`
- `void sort(Comparator<? super E> c)`: sort the list in $O(N\log N)$ time
- `E set(int index, E element)`: Replaces the element at the specified position in this list with the specified element.
- `boolean add(E e)`: Appends the specified element to the **end** of this list.
- `void add(int index, E element)`
- `boolean addAll(Collection<? extends E> c)`
- `boolean addAll(int index, Collection<? extends E> c)`: Inserts all of the elements in the specified collection into this list, starting at the specified position.
- `void forEach(Consumer<? super E> action)`: Performs the given action for each element of the Iterable until all elements have been processed or the action throws an exception.
- `int indexOf(Object o)`: Returns the index of the **first occurrence** of the specified element in this list, or -1 if this list does not contain the element.
- `int lastIndexOf(Object o)`: Returns the index of the **last occurrence** of the specified element in this list, or -1 if this list does not contain the element.
- `E remove(int index)`: Removes the element at the specified position in this list.
- `boolean remove(Object o)`: Removes the **first occurrence** of the specified element from this list, if it is present.
- `boolean removeAll(Collection<?> c)`: Removes from this list all of its elements that are contained in the specified collection.
- `boolean removeIf(Predicate<? super E> filter)`: Removes all of the elements of this collection that satisfy the given predicate.
- `protected void removeRange(int fromIndex, int toIndex)`: Removes from this list all of the elements whose index is between fromIndex, **inclusive**, and toIndex, **exclusive**.
- `List<E> subList(int fromIndex, int toIndex)`: Returns a view of the portion of this list between the specified fromIndex, **inclusive**, and toIndex, **exclusive**.
- `Object[] toArray()`: Returns an array containing all of the elements **in this list** in proper sequence (from first to last element).
- `<T> T[] toArray(T[] a)`: Returns an array containing all of the elements **in this list** in proper sequence (from first to last element); the runtime type of the returned array is that of the specified array.
- `Object clone()`: Returns a shallow copy of this ArrayList instance.
- `void ensureCapacity(int minCapacity)`: Increases the capacity of this ArrayList instance, if necessary, to ensure that it can hold at least the number of elements specified by the minimum capacity argument.

## Reference
- [Javadocs/ArrayList](https://docs.oracle.com/javase/8/docs/api/java/util/ArrayList.html)