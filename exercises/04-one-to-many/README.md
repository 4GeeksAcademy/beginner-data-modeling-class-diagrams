# 04 - One to Many

Spanish version: [README.es.md](./README.es.md)

## Scenario

The library has several branches. Each branch holds many books, but each book is stored at one branch.

## Instructions

1. Add class **`Branch`** with:

| Property | Type |
|----------|------|
| `id` | `int` |
| `name` | `string` |
| `city` | `string` |

2. Draw a **one-to-many (1:N)** relationship: one **`Branch`** has many **`Book`** instances.
3. Label cardinality on both ends (for example `1` on the branch side and `N` or `*` on the book side).

## Checklist

- [ ] `Branch` is modeled with typed properties.
- [ ] Each `Book` links to exactly one `Branch` in your diagram.

## Next step

**05 - Boolean Property** — availability flag on books.
