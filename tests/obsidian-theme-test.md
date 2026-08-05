---
aliases:
  - Lucy visual regression fixture
tags:
  - lucy-theme-test
---

# H1 — Two rails around a long heading that can wrap at narrow editor widths

Click this paragraph above and below the heading to verify that the cursor lands on the selected line.

# H1 with **bold**, *italic*, `inline code`, ==highlight==, and %%a comment%%

## H2 — Underline and original vertical rhythm

### H3 — Accent hierarchy

#### H4 — Accent hierarchy

##### H5 — Accent hierarchy

###### H6 — Accent hierarchy

## Paragraph and blank-line geometry

First paragraph with **bold**, *italic*, ~~strikethrough~~, ==highlight==, `inline code`, and a [[Wiki link]].


Second paragraph after two native-height blank lines. Click each blank line and verify that the caret follows the click.

## Unordered lists

- Level one has enough text to wrap at a narrow editor width so its continuation begins exactly below the first text character.
  - Level two uses a hollow circle and also contains enough text to wrap onto a continuation line.
    - Level three uses a square marker and contains enough text to wrap onto another line.
      - Level four cycles back to a disc.
        - Level five cycles back to a hollow circle.
          - Level six cycles back to a square.
- Short level-one item.
- [ ] Unfinished task item with wrapping text that verifies task-marker and continuation alignment.
- [x] Finished task item.

## Ordered lists

1. First ordered item has enough text to wrap and verify that the continuation aligns with the first text character.
2. Second ordered item.
   1. Nested ordered item with enough text to wrap and verify alignment at the second nesting level.
      1. Third nesting level.
3. Third ordered item.

## Right-to-left lists

- هذه فقرة عربية طويلة لاختبار محاذاة السطر الثاني مع بداية النص في قائمة ذات اتجاه من اليمين إلى اليسار.
- عنصر عربي قصير.

1. هذا عنصر مرقم طويل لاختبار المسافة بين الرقم والنص ومحاذاة الأسطر الملتفة.
2. عنصر مرقم قصير.

## Blockquotes and comments

> A single-line blockquote.
>
> A connected blockquote paragraph with enough text to wrap and confirm that the vertical border remains continuous.

Visible text before %%a highlighted editor comment that should remain readable in light and dark mode%% visible text after.

## Tables

| Left aligned | Centered | Right aligned |
| :--- | :---: | ---: |
| Alpha | Beta | 1 |
| Gamma | Delta | 2 |

## Callouts

> [!note] Accent-synchronized note
> The border, background, title, and icon should follow the custom accent color.
>
> | Embedded table | Value |
> | --- | ---: |
> | Alpha | 1 |

> [!info] Lucy info color
> Verify this callout in both light and dark modes.

> [!todo] Lucy todo color
> Verify this callout in both light and dark modes.

> [!note] Bases embed check
> Point this placeholder at an existing disposable Base in the test vault before checking embedded table colors.
>
> ![[Theme fixture.base]]

## Final cursor target

Click this final paragraph after testing the content above.
