# Java Race Condition Example

This repository demonstrates a classic race condition in a simple Java counter program.  Two threads increment a shared counter concurrently, leading to an inaccurate final count.  The solution showcases how to fix this using proper synchronization techniques.

## Bug
The `Counter` class is not thread-safe. The `increment()` method is not atomic; multiple threads accessing and modifying `count` concurrently can cause data corruption.

## Solution
The solution uses the `synchronized` keyword to ensure that only one thread can access and modify the counter at a time, preventing the race condition.
