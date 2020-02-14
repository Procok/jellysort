# jellysort
A sorting algorithm inspired by eating jelly beans while I was sorting them by colour. 
Trying to make it as fast as possible or to see if it even doable as I imagined it.

How it works? (or how it should)
  In: (Ord a) => [a]
  Out: Ordered [a]
  Space complexity: 2 * n + k ~ O(n), where n is the size of the container and k is the chunk size of the run.
  Time complexity: This should be O(n * logn).
  
  The algorith uses the divide and conquer method. 
  The division is done by choosing smaller and smaller, *mostly* sorted chunks of
  the container and moving them to their place in a temp container.
  Then the overwrite the original with the temp and a new run begins.
  The *mostly* sortedness can be configured as the percent of in order elements to all element of the chunck size. 
  (I will test multiple configurations here. I am not sure what could work the best atm.)
