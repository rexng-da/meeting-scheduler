# Meeting Scheduler

This is a toy Daml project to showcase the Daml's and Canton's capabilities.

## How to run

### Canton

This creates a local Canton service in interactive console mode with 2 participant nodes and 1 domain node.

`canton -c canton/local-memory.conf --bootstrap canton/bootstrap.canton`

You can then examine the ledger API by connecting Daml Navigator to it

`daml navigator server localhost 5011 --feature-user-management=false`

The reason the `--feature-user-management=false` option is set is because we are simplifying here dealing with parties instead of users.
