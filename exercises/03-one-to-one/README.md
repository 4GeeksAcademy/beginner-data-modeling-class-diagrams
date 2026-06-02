# 03 - One to One

Spanish version: [README.es.md](./README.es.md)

## Scenario

Each library member has exactly one membership card, and each card belongs to one member.

## Instructions

1. Add class **`LibraryCard`** with:

| Property | Type |
|----------|------|
| `id` | `int` |
| `cardNumber` | `string` |
| `issuedAt` | `date` |

2. Draw a **one-to-one (1:1)** relationship between **`Member`** and **`LibraryCard`**.
3. Label the relationship ends so it is clear each member has one card and each card belongs to one member.

## Checklist

- [ ] `LibraryCard` exists with typed properties.
- [ ] Cardinality shows **1:1** between `Member` and `LibraryCard`.

## Next step

**04 - One to Many** — books will belong to branches.
