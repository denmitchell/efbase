# EFBase Wiki
The EFBase package provides a SqlServerRepo and SqlServerContext for Entity Framework targeting SQL Server 2016+.  The SqlServerRepo class includes methods for creating, reading (by PK), updating, and deleting -- both synchronously and asynchronously.  The SqlServerRepo class also includes methods for returning JSON from a valid FOR JSON SQL Server SELECT statement.  Finally, SqlServerRepo supports auto-rollback transactions and sequence-resetting, which are useful for testing.  To use SqlServerRepo, be sure to extend both SqlServerRepo (for all of your repository classes) and SqlServerContext (for all of your DbContext subclasses).  The following classes are included:
1. **[SqlServerContext](https://github.com/denmitchell/efbase/wiki/SqlServerContext)** -- which extends DbContext to provide support for FOR JSON queries.
2. **[SqlServerRepo](https://github.com/denmitchell/efbase/wiki/SqlServerRepo)** -- which provides the base repository class.  This class support auto-rollback transactions (for testing purposes).
3. **[SequenceResetter](https://github.com/denmitchell/efbase/wiki/SequenceResetter)**-- which provides a method for resetting all sequences in a database.
4. **[SqlExecutor](https://github.com/denmitchell/efbase/wiki/SqlExecutor)** -- which provides methods for executing multiple SQL statement blocks separated by GO.
5. **[SqlJson](https://github.com/denmitchell/efbase/wiki/SqlJson)** -- which allows Entity Framework to return FOR JSON statements from SQL Server.](https://github.com/denmitchell/efbase/wiki/SqlJson)** -- which allows Entity Framework to return FOR JSON statements from SQL Server.