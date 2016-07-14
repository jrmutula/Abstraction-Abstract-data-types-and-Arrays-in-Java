<h1>Abstract Data Type</h1>

In computer science, an abstract data type (ADT) is a mathematical model for data types where a data type is defined by its behavior (semantics) from the point of view of a user of the data, specifically in terms of possible values, possible operations on data of this type, and the behavior of these operations. This contrasts with data structures, which are concrete representations of data, and are the point of view of an implementer, not a user.

Here are some examples of abstract data types, along with some of their operations, grouped by kind.

<strong>int</strong> is Java’s primitive integer type. int is immutable, so it has no mutators.

1. creators: the numeric literals 0, 1, 2, …
2. producers: arithmetic operators +, -, ×, ÷
3. observers: comparison operators ==, !=, <, >
4. mutators: none (it’s immutable)

<strong>List</strong> is Java’s list interface. List is mutable. List is also an interface, which means that other classes provide the actual implementation of the data type. These classes include ArrayList and LinkedList.

1. creators: ArrayList and LinkedList constructors, Collections.singletonList
2. producers: Collections.unmodifiableList
3. observers: size, get
4. mutators: add, remove, addAll, Collections.sort

<strong>String</strong> is Java’s string type. String is immutable.

1. creators: String constructors
2. producers: concat, substring, toUpperCase
3. observers: length, charAt
4. mutators: none (it’s immutable)

This classification gives some useful terminology, but it’s not perfect. In complicated data types, there may be an operation that is both a producer and a mutator, for example. Some people reserve the term producer only for operations that do no mutation.
