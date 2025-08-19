In a multi-threaded producer-consumer program, verifying correctness means
  1. All produced items are eventually consumed exactly once.
  2. No item is lost or processed multiple times
  3. The program terminates gracefully when all work is done.

How to check correctness?
1. Use a shared counter or collection to track produced and consumed items.
  When a producer creates an item, record it ( eg, add to a Set or increment a counter)
  When a consumer processes an item, record it in a similar manner.
  After processing finishes, compare the two sets or counts

Additional Ideas for correctness:
  Use counters: Atomic counters for produced and consumed counts - check if they match at the end.
  Poison pill or termination signal: ensure consumer threads stop after all work is done.
  Logging: produce logs with item IDs and thread names, then analyze logs post-run
  Concurrency Testing tools: Use specialized tools ( like Java Concurrency Stress tests or libraries like JCStress) to detect concurrency bugs.

For Multiple Consumers and Producers:
1. Make sure all consumers stop after processing all items ( often by sending as many poison pills as consumers)
2. Track itesm globally ( thread-safe collections) and compare at the end.



