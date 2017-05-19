## Intro to Elixir

#### Donald Plummer
#### dplummer@avvo.com

---

What is the Elixir programming language?

---

## Elixir is:
- *functional, immutable*
- *pattern matching*
- *concurrent*
- *fault-tolerant*
- *Erlang virtual machine*
- Modern tooling borrowing from recent languages and frameworks, like Ruby and Rails.

---

## Functional

- Functions are basic building blocks
- Code is organized around transforming data

---

## Immutable

- Objects are not changed
- Code is easier to test
- Makes code thread safe, prevents concurrency bugs

---

## Pattern matching

```elixir
iex> x = 1
1
iex> x
1
```

```
iex> 1 = x
1
iex> 2 = x
** (MatchError) no match of right hand side value: 1
```

---

## Multiple functions heads

```elixir
iex> defmodule M do
...> def foo(1), do: "one"
...> def foo(2), do: "two"
...> def foo(_), do: "I can't count that high"
...> end
iex> M.foo(1)
"one"
iex> M.foo(2)
"two"
iex> M.foo(3)
"I can't count that high"
```

---

## Concurrency

- Runs 100,000s of processes per machine
- Not same as OS processes or threads
- No global interpreter lock (GIL) so will use all processors

---

## Processes

- Long lived
- Sends messages to other processes
- Each has their own mailbox
- Handles one message at a time

---

## Fault tolerance

- Links (two way)
- Monitors (one way)
- Timeouts
- Supervision trees

---

## Supervision trees

- Process that just monitors children
- Can restart child processes if they fail

---

## Erlang virtual machine

- Battle tested by Ericsson
- Runs worlds phone switches, SMS gateways, cell towers

---

## Modern tooling

- Nicer syntax
- Macros
- Inline documentation
- Command line tools
- Open source community

---

## Q & A

---

## Resources
Slides: https://gitpitch.com/dplummer/slides-intro-elixir

Language: http://elixir-lang.org
