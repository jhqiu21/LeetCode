# Array
## API
!!! Note
    Here, I have listed some commonly used *generic* methods. For the complete methods, please refer to [Javadocs](https://docs.oracle.com/javase/8/docs/api/)
### Class `Arrays`
!!! Attention
    All method in class `Arrays` are `static` method!
- `static <T> List<T> asList(T... a)`: Returns a fixed-size list backed by the specified array.
- `static <T> int binarySearch(T[] a, int fromIndex, int toIndex, T key, Comparator<? super T> c)`: Searches a range of the specified array for the specified object using the binary search algorithm.
- `static <T> int binarySearch(T[] a, T key, Comparator<? super T> c)`: Searches the specified array for the specified object using the binary search algorithm.
- `static <T> T[] copyOf(T[] original, int newLength)`: Copies the specified array, truncating or padding with nulls (if necessary) so the copy has the specified length.
- `static <T> T[] copyOfRange(T[] original, int from, int to)`: Copies the specified range of the specified array into a new array.
- `static void fill(Object[] a, int fromIndex, int toIndex, Object val)`: Assigns the specified Object reference to each element of the specified range of the specified array of Objects.
- `static void fill(Object[] a, Object val)`: Assigns the specified Object reference to each element of the
- `static <T> void sort(T[] a, Comparator<? super T> c)`: Sorts the specified array of objects according to the order induced by the specified comparator.
??? Example
    For a 2-d array, sort the array based on the RHS of each 'interval'<br/>
    `Arrays.sort(intervals, (a,b) -> Integer.compare(a[1], b[1]));`

- `static <T> void sort(T[] a, int fromIndex, int toIndex, Comparator<? super T> c)`: Sorts the specified range of the specified array of objects according to the order induced by the specified comparator.
- `static String toString(Object[] a)`: Returns a string representation of the contents of the specified array.
### Class `Array`
- `static Object get(Object array, int index)`: Returns the value of the indexed component in the specified array object.

## Reference
- [Javadocs/Arrays](https://docs.oracle.com/javase%2F8%2Fdocs%2Fapi%2F%2F/java/util/Arrays.html)
- [Javadocs/Array](https://docs.oracle.com/javase%2F8%2Fdocs%2Fapi%2F%2F/java/lang/reflect/Array.html)