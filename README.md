# FlusterIO

![Fluster banner](fluster_banner.png)

> **Tools for thinking, researching, and building with knowledge.**

FlusterIO is building a new kind of academic computing environment: **a local-first, structured knowledge system designed to work with both humans and AI.**

The project began with [Fluster](https://www.flusterapp.com), an academic note-taking application I originally built for my own research. I wanted something that treated notes less like documents and more like a connected body of knowledge — searchable, linkable, extensible, and capable of understanding the structure of the material inside them.

That experiment eventually grew into **Conundrum**.

## The Projects

### [Fluster](https://www.flusterapp.com)

Fluster is the application layer: a native academic workspace built around writing, research, mathematics, diagrams, citations, and connected knowledge.

The upcoming Apple applications are being rebuilt around Conundrum, providing a native interface for the underlying knowledge system.

**Initial capabilities include:**

* Full, multi-page free-draw canvas
* MDX-based editor

  * Component snippets
  * Syntax highlighting
  * Vim support
  * Emacs support
* Structured search

  * Tags
  * Topics
  * Subjects
  * Citations
  * Full-text search
  * Syntax-aware search re-ranking
* Integrated bibliography management
* CSL citation formatting
* Native Apple-platform applications

**The repo you're probably looking for:**

[github.com/flusterIO/fluster-ipad](https://github.com/flusterIO/fluster-ipad)

---

### Conundrum

**Conundrum is the engine underneath Fluster.**

It is a modular academic toolkit and structured knowledge layer designed to make personal data useful to both traditional software and AI systems.

The core idea is simple:

> **Your notes shouldn't have to become context just because an AI needs to understand them.**

Instead of treating a knowledge base as a collection of files that must repeatedly be loaded into a context window, Conundrum maintains structured relationships between pieces of information and exposes those relationships through a programmable ecosystem.

The project is built primarily in **Rust**, with the goal of running across native and WebAssembly environments.

Some of the pieces include:

* A structured, graph-oriented data model
* Local LanceDB-backed storage
* Full-text and structured search
* Vector-search infrastructure
* An MDX-derived knowledge language
* Rust-powered compilation
* MCP integration
* CLI tooling
* Native and WebAssembly support
* SDKs for multiple languages
* AI/RAG integrations
* Procedural macros for reducing database and model boilerplate

Conundrum is intended to be useful independently of Fluster. Fluster is one application built on top of it; the underlying toolkit is meant to be reusable by other applications, agents, and workflows.

---

## A Different Approach to Notes

Most note-taking software starts with the document.

Conundrum starts with the **information**.

A document is one representation of that information. A database record, a graph relationship, a search result, an embedding, an MCP resource, or an AI-generated transformation can be another.

This makes it possible to build workflows where the same knowledge can move between:

**human → note → database → search → AI → computation → visualization → note**

without requiring every system to maintain its own isolated representation.

The long-term goal is an environment where writing a note can be as computationally expressive as writing a small program, without requiring the user to leave the document.

---

## Conundrum Language

Conundrum extends the ideas behind Markdown and MDX into a domain-specific language for structured academic work.

The intention is to preserve the accessibility of Markdown while providing first-class concepts for things such as:

* Mathematics
* Equations and equation identifiers
* References
* Citations
* Structured links
* Components
* Metadata
* Computation
* Search
* Knowledge relationships

Existing MDX should remain familiar wherever possible. Conundrum is intended to feel less like learning an entirely new language and more like discovering that your notes have capabilities you didn't realize were there.

And unlike traditional MDX implementations, the Conundrum toolchain is **Rust-first**. Compilation and core language functionality do not depend on JavaScript or TypeScript.

---

## AI Without Giving Up Your Data

AI systems are extremely good at reasoning over information.

They're considerably less good at reasoning over information that doesn't fit into their context window.

Conundrum is an attempt to address that problem at the data layer.

Rather than repeatedly handing an AI an enormous collection of documents, Conundrum provides structured ways for an agent to discover what information exists, search for relevant material, follow relationships, retrieve specific records, and perform operations against the user's knowledge base.

MCP provides one interface for exposing that capability to AI systems.

The goal isn't to build another chatbot.

The goal is to make **your knowledge programmable**.

---

## Research as a Computing Environment

The long-term vision for Fluster goes beyond note-taking.

I want Fluster to become a Markdown-first, Jupyter-friendly environment where a researcher can move naturally between:

* Writing
* Mathematics
* Code
* Data
* Visualization
* Citations
* Files
* Computation
* AI-assisted research

without turning their research into a collection of disconnected applications.

A future Fluster document should be capable of being simultaneously:

**a paper, a notebook, a database, a computational workspace, and a knowledge graph.**

That's a fairly ambitious goal.

That's also the point.

---

## Why It Exists

Fluster originally existed because I couldn't find the tool I wanted for my own academic work.

I needed something that could keep up with ideas that didn't fit neatly into folders, documents, or conventional notebooks. I wanted to be able to follow connections between concepts, search through years of work, work with mathematics and diagrams, and eventually allow software to reason about the same material.

So I built it.

What started as a personal application eventually became a much larger question:

> **What should a computer-assisted research environment look like if we design it around knowledge rather than documents?**

Fluster and Conundrum are my attempt at an answer.

---

## Where We're Going

The immediate goal is to finish bringing the Conundrum architecture into the native Fluster applications and establish the underlying toolkit as a stable platform.

From there, the roadmap increasingly moves toward:

* Richer computational documents
* Better semantic and vector search
* AI-native knowledge retrieval
* More powerful MCP tooling
* Cross-platform Conundrum applications
* Jupyter interoperability
* Programmable notes
* Native mathematical and scientific workflows
* Extensible knowledge components
* A broader ecosystem of applications built on Conundrum

The project is intentionally being built in layers.

**Conundrum provides the foundation.
Fluster provides the experience.
The ecosystem provides the possibilities.**

---

## The Research Behind It

Fluster was originally created alongside my own work in physics and mathematics.

That research eventually led me to explore an alternative formulation of gravitational and electromagnetic geometry, including a proposed relationship between gravitational parameters and the fine-structure constant.

You can read about that work here:

[On the Gravitational Nature of Time](https://www.flusterapp.com/docs/my_work/on_the_gravitational_nature_of_time)

Whether the physics ultimately survives scrutiny is almost beside the point.

The important thing is that **Fluster was built because doing this kind of work required better tools.**

The software is an attempt to build those tools.

---

## Current Status

Fluster and Conundrum are both actively being developed.

The Apple-specific applications are approaching release, while the underlying Conundrum ecosystem continues to expand.

Some parts of the project are mature.

Some parts are experimental.

Some parts are being rebuilt because I found a better way to do them.

That's intentional.

This is a long-term project, and the architecture is still evolving alongside the problems it's designed to solve.

---

## Contributing

Conundrum is intended to become a platform that other developers can build on.

If you're interested in:

* Rust
* Knowledge graphs
* AI tooling
* MCP
* RAG
* Databases
* Compilers
* MDX
* Scientific computing
* Mathematical software
* Native applications
* Developer tooling

there should eventually be something interesting here for you.

The best place to start is with the individual project repositories and their documentation.

---

## FlusterIO

**Research tools for the next generation of knowledge work.**

**Fluster** is the application.

**Conundrum** is the engine.

**Your knowledge is the data.**

And the ultimate goal is to make that knowledge as computationally useful as everything else on your computer.

---

*Built from a problem I couldn't find a good solution to.*
