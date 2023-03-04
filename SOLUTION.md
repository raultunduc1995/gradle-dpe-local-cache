# Lab 01: Local build cache solution

## Steps
-----
1. **Were the results of any cacheable tasks stored within the cache?**

    To search for tasks resolved from the cache, click the magnifying glass on the Timeline view.
    Set "Task output cacheability" to "Cacheable" and you should see the list of cacheable tasks.

    For this example, the cacheable tasks are `compileJava`, `compileTestJava` and `test`.

    If you look at the expanded view of any of these tasks, you will see that the build cache result is indeed stored in the local cache.

2. **Were there any timesavings due to the cache in these builds?**

    Because there were no cache hits, there were no time savings (called "Avoidance savings" on the scan).
    If you look at the next scan with cache hits, you'll see the avoidance savings right below duration.

3. **Which tasks were resolved from the cache?**

    To find which tasks were resolved from the cache, set the 'Outcome' to `FROM-CACHE` on the Timeline tab.

4. **Were there any cacheable tasks that were not resolved from the cache?**

    Not in this example.

5. **How much faster is the fully cached build than the uncached build?**

    This number will vary based on your environment.
    You will find the answer for your build on the "Performance" tab under 'Task execution'.
