# kotlin vs Java

## Collection Initialization

#### Immutable List
```kotlin
// kotlin
val nums = listOf(1, 2, 3)
```

```java
// Java + Guava
ImmutableList<Integer> nums = ImmutableList.of(1, 2, 3);
```
######P.S. Collections.unmodifiableList(..) is not really immutable.

#### Mutable List
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

#### Empty List
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
#### Immutable Set
```kotlin
// kotlin
val nums = setOf(1, 2, 3)
```

```java
// Java + Guava
ImmutableSet<Integer> nums = ImmutableSet.of(1, 2, 3);
```
######P.S. Collections.unmodifiableSet(..) is not really immutable.

#### Mutable Set
```kotlin
// kotlin
val nums = mutableSetOf(4, 5, 6)
```

```java
// Java + Guava
Set<Integer> nums = Sets.newHashSet(4, 5, 6);
```
#### Empty Set
```kotlin
// kotlin
val nums = emptySet()
```

```java
// Java
Set<Integer> nums = Collections.emptySet();

// Java + Guava
ImmutableSet<Integer> nums = ImmutableSet.of();
```

#### Immutable Map
```kotlin
// kotlin
val map = mapOf(1 to "a", 2 to "b", 3 to "c")
```

```java
// Java + Guava
ImmutableMap<Integer, String> map = ImmutableMap.of(1, "a", 2, "b", 3, "c");
```
######P.S. Collections.unmodifiableMap(..) is not really immutable.

#### Mutable Map
```kotlin
// kotlin
val map = mutableMapOf(4 to "d", 5 to "e", 6 to "f")
```

```java
// Java + Guava
ImmutableMap<Integer, String> map = ImmutableMap.of(1, "a", 2, "b", 3, "c");
```

#### Empty Map
```kotlin
// kotlin
val map = emptyMap()
```

```java
// Java + Guava
ImmutableMap<Integer> map = ImmutableMap.of();
```
