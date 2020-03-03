# GenServer with supervision tree and state recovery after crash

You’ve probably heard that in Elixir you should let processes crash
rather than trying to catch every possible exceptions. Then, after a
crash, you only have to get back to the latest good known state in the
process the supervisor created for you. Great but there are few
explainations about how to recover the state available out there.

Let’s fix this!

## Read the blog post

[GenServer with supervision tree and state recovery after crash](https://www.bounga.org/elixir/2020/02/29/genserver-supervision-tree-and-state-recovery-after-crash/)

## Run the example code

```sh
mix deps.get
iex -S mix
```

Then play in the REPL:

```iex
Sequence.Server.next_number()
Sequence.Server.increment_number(12)
Sequence.Server.next_number()
```
