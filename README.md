# MicrosoftADC_Assignment2

## Question
#### Write a function that returns the first non-duplicated character in a string. For example, the string, "minimum" has two characters that only exist once—the "n" and the "u", so your function should return the "n", since it occurs first. The function should have an efficiency of O(N)
#### Answer

    string = "minimum"
    l = []
    for i in string:
        if i not in l:
            l.append(i)
            print(l)
        elif i in l:
            l.remove(i)
            print(l)

    print(l)      
    print(l[0])

#### Pro Question: Implement a map using hash table
#### Answer
    array = [5,17,9,5,3]
    key1 = "age"
    key2 = "day"
    key3 = "month"

    maps = {}
    maps.update({key1:array[1]})
    maps.update({key2:array[0]})
    maps.update({key3:array[4]})

    print(maps)

#### Implement heap data structure 
#### Answer
      def heapify(arr,i):
        n = len(arr)
        largest = i
        l = 2 * i + 1
        r = 2 * i + 2 

        if l < n and arr[i] < arr[l]:
            largest = l

        if r < n and arr[largest] < arr[r]:
            largest = r

        if largest != i:
            arr[i],arr[largest] = arr[largest],arr[i]
            heapify(arr)
 #### Similarities and differences between queues, priority queue, and heap data structure? 
 
                   """ Differences
                        A queue the first in first out is a the method of manipulating data,
                        A prority queue each data is given a prority number; the data with the highest priority is handled first. 
                        A heap is an unsorted priority queue that takes the minimum or maximum priority element and stored as the root

                    """
                    """ Similarities
                        The queue, the heap and priority queue data structures all have who they attend to first
                         queue by who comes first
                         priority queue by the highest priority
                         heap by the minimum or maximum number on the node

                    """


