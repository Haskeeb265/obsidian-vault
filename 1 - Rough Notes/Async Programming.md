
2025-11-19 11:50

Status: #Finished

Tags: [[programming]]

# Async Programming

- **Event Loop**:
Runs and schedules coroutines.
Switch tasks and hit await
Handle callbacks and timeouts and I/O events
Resume tasks when awaited operation finishes
Manages all the coroutines

	- Event loop first picks a task to run.
	- The task runs until the event loop encounters the "await" keyword
	- The event loop pauses the task and registers "what" the task is waiting for
	- When the await is finished, mark the task as ready again
	- Repeat

Here's how event loop works:
1. A future is created
2. The selector tells the event loop to lookout for the future (giving it an FD)

Asyncio helps us achieve concurrency. Not parallelism

- **Coroutine**:
An async function is called a coroutine


- await asyncio.gather( tasks, return _exceptions_=True) allows the program to continue and not crash even if one of the many coroutines fails.
- Without this, the whole program would crash even if a single coroutine fails


- Python is not a multithreaded language

#### References
