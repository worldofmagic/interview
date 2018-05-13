# Java Basic Knowledge

## Thread Pools

A thread pool is a group of threads initially created that waits for jobs and executes them. The idea is to have the threads always existing, so that we won't have to pay overhead time for creating them every time. They are appropriate when we know there's a stream of jobs to process, even though there could be some time when there are no jobs.

![](/assets/import.png)



## Connection Pools

Creating a network connection to a database server is \(relatively\) expensive. Likewise asking the server to prepare a SQL statement is \(relatively\) expensive.

Using a connection/statement pool, you can reuse existing connections/prepared statements, avoiding the cost of initiating a connection, parsing SQL etc.

Performance. Connecting to the database is expensive and slow. Pooled connections can be left physically connected to the database, and shared amongst the various components that need database access. That way the connection cost is paid for once and amortized across all the consuming components.

1. Performance. Connecting to the database is expensive and slow. Pooled connections can be left physically connected to the database, and shared amongst the various components that need database access. That way the connection cost is paid for once and amortized across all the consuming components.

2. Diagnostics. If you have one sub-system responsible for connecting to the database, it becomes easier to diagnose and analyze database connection usage.

3. Maintainability. Again, if you have one sub-system responsible for handing out database connections, your code will be easier to maintain than if each component connected to the database itself.



