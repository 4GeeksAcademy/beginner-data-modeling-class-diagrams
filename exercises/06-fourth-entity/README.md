# 06 - Fourth Entity

Spanish version: [README.es.md](./README.es.md)

## Scenario

Books are written by authors. Model authorship as its own entity.

## Instructions

1. Add class **`Author`** with:

| Property | Type |
|----------|------|
| `id` | `int` |
| `fullName` | `string` |
| `country` | `string` |

2. Connect **`Author`** and **`Book`** with a sensible relationship (for example one author writes many books, or many authors collaborate on many books). Label cardinality on both ends.

## Checklist

- [ ] `Author` has three typed properties.
- [ ] `Author` is related to `Book` with clear cardinality labels.

## Next step

**07 - Many to Many** — members borrow books through a loan record.
