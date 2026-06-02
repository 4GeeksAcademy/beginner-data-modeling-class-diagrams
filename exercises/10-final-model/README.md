# 10 - Final Model

Spanish version: [README.es.md](./README.es.md)

## Congratulations

You finished the guided practice. Compare your [diagram.4geeks.com](https://diagram.4geeks.com/) model with the reference below. Names and layout may differ; focus on **entities**, **typed properties**, and **cardinalities** (1:1, 1:N, N:M).

Mark this LearnPack practice as **complete** when you are satisfied with your diagram.

## Reference solution (Mermaid)

This is one valid way to represent the digital library from steps 01–09:

```mermaid
classDiagram
    class Book {
        int id
        string title
        string isbn
        boolean isAvailable
    }
    class Member {
        int id
        string name
        string email
    }
    class LibraryCard {
        int id
        string cardNumber
        date issuedAt
    }
    class Branch {
        int id
        string name
        string city
    }
    class Author {
        int id
        string fullName
        string country
    }
    class Loan {
        int id
        date loanDate
        date dueDate
    }
    Member "1" --> "1" LibraryCard : has
    Branch "1" --> "*" Book : holds
    Author "1" --> "*" Book : writes
    Member "1" --> "*" Loan : borrows
    Loan "*" --> "1" Book : for
```

## Relationship summary

| From | To | Type | Notes |
|------|-----|------|-------|
| `Member` | `LibraryCard` | 1:1 | One card per member |
| `Branch` | `Book` | 1:N | One branch, many books |
| `Author` | `Book` | 1:N | One author, many books (simplified) |
| `Member` | `Book` | N:M | Through `Loan` |

## What to do next

- Export a PNG from diagram.4geeks.com for your portfolio if you want.
- Continue with the [data modeling and class diagrams](https://github.com/4GeeksAcademy/data-modeling-and-class-diagrams) project for full deliverables.

## Discussion questions

1. Could `Loan` store a `returnedAt` date? How would that change the model?
2. If a book has multiple authors, how would you adjust the `Author`–`Book` relationship?
3. Why use an association class for borrowing instead of a direct link between `Member` and `Book`?
