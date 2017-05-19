# Intro to Elixir presentation

* Elixir is a *functional, immutable*, programming language for building *concurrent* and
  *fault-tolerant* applications. It is built on the *Erlang virtual machine*, but borrows many
  concepts from more *recent developments*, especially from Ruby.
* As a functional language, code is organized around transforming data from one form to another
  using functions.
* Being immutable, no data is mutated, which makes it easier to test, and makes it thread safe
  (bonus for concurrency)
* Speaking of concurrency, Elixir is built to run thousands to hundreds of thousands of concurrent
  processes on a single machine. These "processes" are internal objects, run by the virtual
  machine's scheduler. They are not system processes or threads. If your machine has multiple
  cores, it will be highly parallel too, running code on all every processor.
* Being built on the Erlang virtual machine, Elixir has many tools for building fault tolerant
  applications: process links (two way), monitors (one way), timeouts, exit trapping, process
  naming, and supervision trees. There are many gotchas in how to set these up to avoid race
  conditions or to always remember a process could die at any time. OTP is a collection of
  libraries and standards for building servers and supervisors the right way. These are battle
  tested, industry standard methodologies that run the world's phone switches, SMS gateways, and
  cell towers.
* While Elixir is built on the Erlang virtual machine, and enjoys full interoperability with
  Erlang libraries, it adds several important features: a nicer syntax, macros, built-in
  documentation, command line tools, and an open source community.
