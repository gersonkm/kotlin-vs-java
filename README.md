# kotlin-vs-java

## Collection Initialization

#### Immutable
```kotlin
// kotlin
val nums = listOf(1, 2, 3)
```

```java
// Java + Guava
ImmutableList<Integer> nums = ImmutableList.of(1, 2, 3);
```
P.S. Collections.unmodifiableList(..) is not really immutable.

#### Mutable
```kotlin
// kotlin
val nums = mutableListOf(4, 5, 6)
```

```java
// Java
List<Integer> nums = Arrays.asList(1, 2, 3);

// Java + Guava
List<Integer> nums = Lists.newArrayList(4, 5, 6);
```

#### Empty
```kotlin
// kotlin
val nums = emptyList()
```

```java
// Java
List<Integer> nums = Collections.emptyList();

// Java + Guava
ImmutableList<Integer> nums = ImmutableList.of();
```
