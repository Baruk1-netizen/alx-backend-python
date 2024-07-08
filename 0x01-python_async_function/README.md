# Async Python Functions

This repository demonstrates the basics of asynchronous programming in Python using the `asyncio` library. Below is a detailed description of each module and its functionality.

## 0. The Basics of Async

This module introduces the concept of asynchronous coroutines. It contains a coroutine named `wait_random` that takes an integer argument `max_delay` (default value of 10). The coroutine waits for a random delay between 0 and `max_delay` seconds and then returns the actual delay.

## 1. Execute Multiple Coroutines Simultaneously

This module demonstrates running multiple coroutines concurrently. It imports the `wait_random` coroutine from the previous module and defines an async routine called `wait_n`. This routine takes two integer arguments, `n` and `max_delay`, and spawns `wait_random` `n` times with the specified `max_delay`. It returns a list of all the delays in ascending order.

## 2. Measure the Runtime

This module focuses on measuring the execution time of concurrent coroutines. It imports the `wait_n` coroutine and defines a function `measure_time` that takes integers `n` and `max_delay` as arguments. This function measures the total execution time for `wait_n(n, max_delay)` and returns the average time per coroutine.

## 3. Tasks

This module explores creating asyncio tasks. It imports the `wait_random` coroutine and defines a function `task_wait_random` that takes an integer `max_delay` and returns an `asyncio.Task` object.

## 4. Tasks (Extended)

This module extends the concept of asyncio tasks. It alters the `wait_n` function to create a new function `task_wait_n`, which uses `task_wait_random` to create tasks instead of directly awaiting coroutines. The functionality is similar to `wait_n` but leverages tasks for concurrency.

## Repository

- **GitHub repository**: `alx-backend-python`
- **Directory**: `0x01-python_async_function`

This repository contains the implementation of the concepts outlined above, providing a hands-on approach to learning asynchronous programming in Python.

##AUTHOR
@Baruk1-netizen
