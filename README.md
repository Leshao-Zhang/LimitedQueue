# LimitedQueue
Generic LimitedQueue for Java, iteratable

Usage:
~~~~
   LimitedQueue<T> limitedQueue = new LimitedQueue<T>(size);

   limitedQueue.add(T);//add new item;

   limitedQueue.get(i);//get the ith item;

   for(T t:limitedQueue){
     //iterate the queue;
   }
~~~~
  
  Take String array as example:
  
    LimitedQueue<String[]> limitedQueue = new LimitedQueue<String[]>(10);
  
  
  
  This created a queue for Stirng array, the size of queue is 10.
  
  We can simple add new item with:
  
    String[] strArr= {"a","b","c"};
    limitedQueue.add(strArr);
    
    
    
  If we add more than 10 items to the queue, the first few items that over the limit is removed.
  
  We can get the ith item in the queue with:
  
    limitedQueue.get(i);
    
    
    
  We can iterate the queue with advance for loop:
  
    for(String[] strArr:limitedQueue){
       //do something;
    }
    
