# Heapsort
Variant Of Heapsort: 
In the first step it also builds a max-heap. 
In the second step, it also proceeds as the Heap Sort does, but
instead of calling MAX-HEAPIFY , it always floats the new root all the way down to a
leaf level. Then, it checks whether that was actually correct and if not fixes the max-heap by
moving the element up again. This strategy makes sense when considering that the element
that was swapped to become the new root is typically small and thus would float down to a
leaf level in most cases. Hence, one would save the additional tests when floating down the
element. And, the fixing step (moving the element upwards again) would be a rare case.

To Run: g++ -Wall -o heapsort heapsortb.cpp
