# Dataset
Creating functions that would perform logical operations on a pair of Sets (AND, OR, SUBTRACT), additioanlly it would add or  remove elements, or see if elements were in the set.

#Technical Description 

This program was coded in C.

This program also uses the **heap** to allocate space for the Sets

Memory leaks were identified and taken care of using **Valgrind**.

Set is a struct, that contains an array of elements and the length of the array

#Modules 


###**Checking if element x is in the Set**

Pass the Set and the element that needs to be checked 
```C
bool isMemberSet(const Set* self, int x)
```
  
###**Inserting an element**

In order to insert an element into a set, pass the Set and the element. It will only be added if the element is not already in the Set.

```C
void insertSet(Set* self, int x)
```

###**Removing an element**

This function will remove an element only if the element is in the set.

```C
void removeSet(Set* self, int x)
```



###**Checking if two sets are equal**

Return true if the two sets are equal.

```C
bool isEqualToSet(const Set* self, const Set* other)
```

###**Check if two sets are subsets of each other (if every element of self is in other)**

```C
isSubsetOf(const Set* self, const Set* other)
```

###**Remove all elements from self that are not also elements of other**

```C
void intersectFromSet(Set* self, const Set* other)
```

###**Remove all elements from self that are also elements of other**

```C
void subtractFromSet(Set* self, const Set* other)
```

###**Add all elements of other to self without creating duplicate elements**

```C
unionInSet(Set* self, const Set* other)
```

