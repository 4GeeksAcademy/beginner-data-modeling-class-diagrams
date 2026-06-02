# 08 - Typed Properties Review

Spanish version: [README.es.md](./README.es.md)

## Scenario

Each loan records when the book was borrowed and when it is due back.

## Instructions

Extend **`Loan`** with:

| Property | Type |
|----------|------|
| `loanDate` | `date` |
| `dueDate` | `date` |

Review your diagram and confirm you are using these types consistently:

- `int` — identifiers and counts
- `string` — names, codes, email
- `boolean` — flags such as `isAvailable`
- `date` — calendar fields such as `issuedAt`, `loanDate`, `dueDate`

## Checklist

- [ ] `Loan` includes both `date` properties.
- [ ] At least four distinct classes remain on the canvas.
- [ ] Every property in the diagram shows an explicit type.

## Next step

**09 - Complete Model** — polish the full library diagram.
