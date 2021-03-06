# Listeners : What are conflict listeners and how to work with them?

To allow users to handle document replication conflicts automatically, we introduced a Document Conflict listener.
To create your own listener of this type, just implement IDocumentConflictListener interface.

{CODE:java document_conflict_listener@ClientApi\Listeners\Conflict.java /}

##Example

This example shows how to create an automatic conflict resolver by using `IDocumentConflictListener`, which will pick the newest item from the list of conflicted documents:

{CODE:java document_conflict_example@ClientApi\Listeners\Conflict.java /}

## Related articles

- [Server : Replication : Conflicts](../../server/scaling-out/replication/replication-conflicts)