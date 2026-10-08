# CSCI161-CH07-EXAMPLES
Examples from Chapter 7 of Data Structures and Algorithms in Java

## Code Fragment 7.1: List Interface
Defines the generic `List<E>` interface for an index-based sequence. Includes methods for checking the size, accessing and replacing elements, and inserting or removing elements at a specified index.

## Code Fragment 7.2: ArrayList Implementation
Implements the list interface using an array. Demonstrates index validation, direct access to elements, and shifting elements during insertion and removal. This initial version uses a fixed-capacity array; resizing is introduced later in the chapter.

## Code Fragment 7.8: PositionalList Interface
Defines the generic `PositionalList<E>` interface. Instead of using numeric indices, operations use `Position<E>` objects to locate elements, navigate between neighbors, and insert, replace, or remove elements.

## Code Fragments 7.9-7.12: LinkedPositionalList Implementation
Together, these fragments implement a positional list using a doubly linked list with header and trailer sentinels. They define the internal node structure, validate positions, provide navigation methods, and implement insertion, replacement, and removal. Given a valid position, updates modify neighboring links rather than shifting elements.

## Code Fragment 7.13: ArrayList Iterator
Adds an iterator to the array-based list. The iterator tracks its progress through the elements and supports `hasNext()`, `next()`, and `remove()`. The list's `iterator()` method creates a new iterator for each traversal.

## Code Fragment 7.15: Insertion Sort for a Positional List
Sorts a positional list of integers in ascending order. Builds a sorted portion of the list and moves each out-of-order element into the correct position by navigating backward through positions.

## Code Fragment 7.17: FavoritesList Public Methods
Provides the public operations for a list that tracks access frequencies. Accessing an element increases its count and maintains the frequency-based ordering. Also supports removing elements and retrieving the most frequently accessed elements.

## Code Fragment 7.18: Move-to-Front Favorites List
Defines `FavoritesListMTF`, a variation that moves each accessed element to the front rather than maintaining frequency order. Access counts are still recorded, but retrieving the most frequently accessed elements requires selecting them by count instead of simply taking the first entries.
