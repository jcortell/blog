---
id: 7094
title: Learning quantum computer programming
date: 2014-05-23T11:05:59+00:00
author: Jorge Cortell
layout: post
guid: https://blog.cortell.net/?p=7094
permalink: /blog/2014/05/23/learning-quantum-computer-programming/
categories:
  - Geek Fun
  - General
  - Hacking
  - "Life's pleasures"
  - Personal
  - Technology
  - Technolust
  - Why not? Utopia?
---
Yesterday I started learning and experimenting with quantum computing programming. It`s not easy to express the fun and excitement that experience brought me, but I`ll try:

<img class="aligncenter" src="https://www.extremetech.com/wp-content/uploads/2014/05/quantum-playground-640x353.jpg" alt="quantum computing simulator" width="640" height="353" />

Programming a quantum computer is different than programming a binary (0 and 1) "digital" computer. To program a quantum system, you have to map a problem into a search for the “lowest point" in a very large pool of options, which corresponds to the best possible outcome. The processor considers all the possibilities simultaneously to determine **the lowest energy required to form those relationships**. A quantum computer is probabilistic rather than deterministic, so the computer returns the best answers in a short amount of time. This results not only in the optimal solution or a single answer, but also other alternatives to choose from.

> Of course, I don`t have access to a quantum computer (_yet_), so I used a GPU-accelerated quantum computer simulator with a simple IDE interface, its own scripting language with debugging, and 3D quantum state visualization which can efficiently simulate quantum registers up to 22 qubits, run Grover`s and Shor`s algorithms, and has a variety of quantum gates built in.

To use the quantum computer you map the problem to an equation whose objective is to return the minimal values (optimal solutions). There are two values that must be provided – the "weights" of the **qubits** (which can exist in any superposition of states 0 and 1, and are represented by a complex number) and the "strengths" of the interaction between them. When N qubits are in superposition, a combination of 2^N states is created.

**Quantum gates** are similar to the logical gates used in binary digital computers. With quantum gates (which define the most basic operations performed on qubits)  you can build complex algorithms, that usually end in a measurement operation obtaining a classical value of qubits (either 0 or 1, but not a superposition).

A set of qubits called **quantum register**, can be visualized in a number of ways, typically as a 2D or 3D graph, on which points or bars represent the "**weight**" superpositions of qubits, while their color or bar height represent the "**strength**" (amplitude and phase) of a given superposition.

> An interesting property of quantum gates is their reversibility, allowing for program execution both forward and in reverse without any side-effects.

The problem is no longer getting an answer, but asking the right question.

Natural Language Processing, Cognitive Computing, Quantum Computing... if you don`t want to fear your rapidly approaching new overlords, better start learning and programming them NOW.

_AI is coming_

&nbsp;