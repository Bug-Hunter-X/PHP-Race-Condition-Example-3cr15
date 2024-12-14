# PHP Race Condition Example

This repository demonstrates a simple race condition in PHP. Two scripts attempt to increment a counter in a file simultaneously, leading to potential data loss and inconsistent results. The solution demonstrates how to avoid race conditions using file locking.

## Bug
The `raceCondition.php` file showcases the race condition. Running multiple instances concurrently will likely result in an incorrect final counter value.

## Solution
The `raceConditionSolution.php` file demonstrates a solution to the race condition using `flock()` for file locking, ensuring exclusive access and preventing data corruption. 