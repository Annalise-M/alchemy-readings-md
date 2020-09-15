Reading notes CT-06: 

    Redis
        @ https://aws.amazon.com/redis/
---
    Redis
        stands for Remote Dictionary Server, is a fast, open-source, in-memory key-value data store for use as a database, cache, message broker, and queue.
---
    Queue
        @ https://www.educative.io/edpresso/what-is-a-queue
---
    A queue is another common data structure that places elements in a sequence, similar to a stack. A queue uses the FIFO method (First In First Out), by which the first element that is enqueued will be the first one to be dequeued.

                Basic operations of a queue
    Enqueue() — Inserts an element to the end of the queue

    Dequeue() — Removes an element from the start of the queue

    isEmpty() — Returns true if queue is empty

    Top() — Returns the first element of the queue

---
    Task Queue Overview
        @ https://redislabs.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/

    Task Queue 
        when we defer operations by putting information about our task to be performed inside a queue, which we process later.

---
    Task Queue - FIFO
        @ https://redislabs.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/6-4-1-first-in-first-out-queues/

    First In First Out Queue (FIFO)
        standard practice with queues (just how it sounds - down the line queue).

---
    Bull Quick Start
        @ https://optimalbits.github.io/bull/

    Bull
        is a Node library that implements a fast and robust queue system based on redis. This library provides an API that takes care of all the low-level details and enriches Redis basic functionality so that more complex use-cases can be handled easily when implementing queues.
