# 07 - Many to Many

Spanish version: [README.es.md](./README.es.md)

## Scenario

A member can borrow many books over time, and a book can be borrowed by many members (on different dates). Model that **many-to-many** pattern with an association class.

## Instructions

1. Add class **`Loan`** (association) with at least:

| Property | Type |
|----------|------|
| `id` | `int` |

2. Link **`Member`** and **`Book`** through **`Loan`** so the relationship is **many-to-many (N:M)**:
   - One member can have many loans.
   - One book can appear in many loans.

3. Label cardinalities along the paths `Member` — `Loan` — `Book`.

## Checklist

- [ ] `Loan` exists between `Member` and `Book`.
- [ ] Cardinality reflects **N:M** borrowing history.

## Next step

**08 - Typed Properties Review** — add dates on `Loan`.
