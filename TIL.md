# TIL this
## Q1  Why do you need SQL when you can use Java or C++ for data manipulation?
    
        # 1 
 -You could store data in Java or CSS sure. Though that might work for making a school project, Facebook cannot store it's user info in that kind of environment. Honestly you don't need to even get that big.It's just what SQL is designed for. Therefore, it does it quicker, better, safer etc.. A knife is for cutting but when I don't have a screwdriver, I've used a knife sometimes.
That might work for one screw on your watch, but that knife can't replace your screw forever. Plus it will take longer, and you will strip the head.

        # 2
-You're absolutely right that you can arrange data in ascending order, find the biggest value, and stuff like that just as easily in Java or C++.

Keep in mind that people rarely use a database just to access existing data. The real power of a database is when you're adding data and modifying data, in addition to accessing it. That's when databases start doing things that'd be a real pain in the ass to do in Java or C++.

So what does a database give you?

Robustness. Suppose you're trying to upload a bunch of data and the power goes out halfway through. Is the whole database corrupt now? With any decent database, your data integrity will be fine and you can continue where you left off.

Simultaneous users. Lots of people can all simultaneously add and modify rows in the database without worrying about anyone overwriting someone else's changes.

Scalability. Your database can be much larger than what fits in RAM. It can even span multiple computers. It's not at all easy to write a Java or C++ program that handles that much data.

So that's why you have a database. The thing is, once you've bought into a database, it's far more efficient to make the database do the work for you when you have a query. So if someone asked "which customer in the database who's been active in the past 30 days has the lowest account balance", sure you could access all of the employees one at a time from Java and then compute the one that matches - but if you know SQL, it will be much faster and more efficient to just ask the database to give you that answer.

## Q2 Why Cache memory is called static RAM , is cache memory type of RAM?

    # 1
Cache memory is a chip-based computer component that makes retrieving data from the computer's memory more efficient. It acts as a temporary storage area that the computer's processor can retrieve data from easily. This temporary storage area, known as a cache, is more readily available to the processor than the computer's main memory source, typically some form of DRAM.

Cache memory is sometimes called CPU (central processing unit) memory because it is typically integrated directly into the CPU chip or placed on a separate chip that has a separate bus interconnect with the CPU. Therefore, it is more accessible to the processor, and able to increase efficiency, because it's physically close to the processor.

In order to be close to the processor, cache memory needs to be much smaller than main memory. Consequently, it has less storage space. It is also more expensive than main memory, as it is a more complex chip that yields higher performance.
