# Java Basic Collection Practice

/
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
2. Why the test failed at first?
3. Why you corrected the test that way?
4. Do you have further questions on this knowledge point?
/

## ArrayTest

should_resize_array
1. The test teaches the characteristics of arrays, most importantly, that it has a fixed size. It also teaches how to instantiate arrays, how to assign values to the elements of an array and how to retrieve the values from an array.
2. The test failed because the pop and push methods were not implemented.
3. The test involved a scenario where an array must have a dynamic number of elements. However, arrays can only a have fixed number of elements. To work around this limitation, the solution involves creating a new array with the increased size. To retain the contents of the old array, a temporary array must be created to hold the values.
4. No.

## CollectionsTest

should_go_through_an_iterator
1. The test teaches how to use an iterator to iterate through elements in a list and retrieve them.
2. The test failed because the method that returns the list created from the passed iterator had no implementation.
3. The hasNext() method returns true while there are elements in a list and the next() method returns the next method in the list and moves the pointer of the iterator through the next element. With these two methods, it is simple to construct a while-loop that adds elements from a list's iterator to another list.
4. No.

should_create_a_sequence_without_putting_all_items_into_memory
1. The test teaches how to create a pseudo-Iterator, and the concept of cursors.
2. The methods were not implemented.
3. Because the output only requires incrementing integers, the implementation I used also involves the use of simple incrementation of integers.
4. No.

should_generate_distinct_sequence_on_the_fly (Did not solve)
1.
2.
3.
4.

should_reflects_back_to_original_list_for_sub_range
1. The use of the subList() method of List objects and how mutating it changes the original list.
2. The expected value is intentionally wrong.
3. The subList(x, y) method returns the items of the List from index x up to, but excluding, index y which would be (3, 4, 5, 6, 7, 8, 9). Because the subList is then cleared, these items are removed from the original list, so the remaining items would be (0, 1, 2, 10, 11).
4. No.