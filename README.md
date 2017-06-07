# A simple C thread pool implementation
### Currently, the implementation:
* Works with pthreads only, but API is intentionally opaque to allow other implementations (Windows for instance).
* Starts all threads on creation of the thread pool.
* Reserves one task for signaling the queue is full.
* Stops and joins all worker threads on destroy.

## Possible enhancements
