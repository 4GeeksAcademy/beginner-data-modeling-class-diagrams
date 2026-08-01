<!-- hide -->

<div align="center">

# Beginner Data Modeling with Class Diagrams

<a href="https://4geeks.com"><img src="https://img.shields.io/badge/4Geeks_Academy-certified-2563eb?style=flat-square" alt="Certified by 4Geeks Academy" /></a>
<a href="https://github.com/learnpack/learnpack"><img src="https://img.shields.io/badge/runs_on-LearnPack-2563eb?style=flat-square" alt="Runs on LearnPack" /></a>
<a href="https://github.com/codespaces"><img src="https://img.shields.io/badge/start-open_in_Codespaces-fb5a1f?style=flat-square&logo=github&logoColor=white" alt="Open in Codespaces" /></a>

</div>

> By [@ehiber](https://github.com/ehiber) and contributors at [4Geeks Academy](https://4geeksacademy.com/)

*These instructions are also available in [Spanish](./README.es.md).*

**Before you start**:

> We need you. These exercises are built and maintained collaboratively by people like you. If you find any typo or mistake, please contribute and/or report it.

<!-- endhide -->

Guided practice in **UML class diagrams** and **data modeling**: **10 steps, about 2 hours**, in which you build one cumulative model for a digital library. You add a class at a time and connect them with real relationships — one-to-one, one-to-many and many-to-many — using [diagram.4geeks.com](https://diagram.4geeks.com/). No setup and no code: you model, you do not program.

## 🎯 What will you learn?

1. How to turn a described scenario into **classes with typed properties** (`int`, `string`, `boolean`, `date`).
2. How to tell the three relationship types apart and when each one is correct: **one-to-one (1:1)**, **one-to-many (1:N)** and **many-to-many (N:M)**.
3. How to resolve a many-to-many relationship with an **association class**, the pattern behind almost every join table you will meet in a database.
4. How to read and write **cardinality** on a diagram, so the model says exactly what the business rule says.
5. How a data model grows without breaking: each step adds to the previous one, which is how real schemas evolve.

## 👀 What will you build?

One model of a **digital library**, built up across ten steps:

1. **First entity** — the `Book` class with typed properties.
2. **Second entity** — a second class, so you have something to relate.
3. **One to one** — a 1:1 relationship and when it is justified.
4. **One to many** — `Branch` and its books: each branch holds many, each book sits in one.
5. **Boolean property** — modelling state, not just data.
6. **Fourth entity** — the model starts to look like a real system.
7. **Many to many** — `Member`, `Book` and the `Loan` association class between them.
8. **Typed properties review** — going back over every class to get the types right.
9. **Complete model** — all the entities and relationships together.
10. **Final model** — compare yours against the reference diagram.

## 🎓 What do you need before starting?

Nothing technical. You do **not** need to know how to program, you do **not** need a database, and you do **not** need to install anything: the whole practice happens in your browser.

It helps to understand what a *table* and a *field* are, but the exercises explain each concept as it appears.

## 📐 How do you check your work?

**This package has no automated tests and nothing to hand in.** There are no answer files or rubrics in the repository either.

Each step describes exactly which classes, properties and relationships your diagram must have, and step **10 - Final Model** contains a reference `classDiagram` to compare against. If your model matches it, you got it right.

> 💡 Comparing your diagram with the reference is more useful than getting it right first time. Where they differ, ask yourself which of the two better describes the scenario in the text.

## 💡 What mistakes should you avoid?

- **Do not model a relationship as a property.** If a book belongs to a branch, that is a relationship between the two classes, not a `branch_name` field inside `Book`. This is the most common beginner error.
- **A many-to-many almost never stays as it is.** As soon as the relationship itself needs data — the date of a loan, for instance — you need an association class in the middle. That is exactly what `Loan` is for in step 07.
- **Cardinality is a business rule, not decoration.** Writing 1:N when the reality is N:M produces a model that cannot store what actually happens.
- **Type every property from the start.** `id` as `int` and `isbn` as `string` is not a detail: it is what will later decide the column type in the database.
- **Do not jump steps.** Each step assumes you modelled the previous concepts. You can move around in LearnPack, but the model is cumulative.

## ❓ Frequently asked questions

### What is a UML class diagram used for?

To describe the structure of a system before building it: which entities exist, which data each one holds and how they relate. It is the step between "the client explained what they need" and "I create the database tables".

### Do I need to know how to program to model data?

No. Modelling is a design activity: you decide what entities exist and how they connect. This practice is done entirely in a diagram tool, without writing a single line of code.

### What is the difference between one-to-many and many-to-many?

In one-to-many each record on one side connects to several on the other, but not the reverse: a branch holds many books, and each book is at one branch. In many-to-many both sides can connect to several: a member borrows many books and a book is borrowed by many members. The second case normally needs an intermediate class to hold the relationship's own data.

### How long does this practice take?

About 2 hours across 10 steps, at your own pace. There is no automatic grading, so you decide when each step is done.

### What tool do I need?

[diagram.4geeks.com](https://diagram.4geeks.com/), which runs in the browser and needs no installation. Keep a single diagram open for the whole practice, since the model is cumulative.

<!-- hide -->

## 🚀 How to start

1. Open this repository in [GitHub Codespaces](https://github.com/codespaces).
2. Wait for the environment to finish setup (LearnPack `5.0.348` is installed automatically).
3. Run:

```bash
learnpack start
```

4. Open [diagram.4geeks.com](https://diagram.4geeks.com/) in your browser and keep one diagram open for the whole practice.

## 📚 How the exercises are organized

Each step folder contains only:

- `README.md` — instructions in English
- `README.es.md` — instructions in Spanish

There are no answer files, tests, or rubrics in this repository.

Steps `01` through `10` build on each other. You can jump between steps in LearnPack, but later steps assume you already modeled earlier concepts.

<!-- endhide -->
