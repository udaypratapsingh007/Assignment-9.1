# Assignment 9.1 - Convert a Desktop Page into a Mobile-First Layout

## Starting Point

I used the dashboard from Week 8 (Assignment 8.4) and rewrote the CSS in a mobile-first way.

## Viewport Meta Tag

The head of index.html has this tag, which makes the page fit the width of the device:

<meta name="viewport" content="width=device-width, initial-scale=1.0">

## Mobile First

The default CSS is written for small screens:

- The dashboard is one column, with the header, sidebar and main content stacked.
- The sidebar links wrap in a row.
- The four statistic cards are in one column.

Larger screens are handled with min-width media queries that add to the mobile styles.

## Breakpoints

- 600px and up (tablet): the header becomes a row, the padding increases and the cards change to 2 columns.
- 900px and up (desktop): the layout becomes a two-column grid with a fixed sidebar of 220px on the left, and the cards change to 4 columns.

## Overflow and Overlap Fixes

- The table is placed in a .table-wrapper with overflow-x: auto, so on a narrow screen only the table scrolls and the page does not scroll sideways.
- The main area has min-width: 0, so wide content cannot push the grid wider than the screen.
- Images use max-width: 100%.

## Testing

I tested the page with Device Mode in Chrome DevTools at mobile, tablet and desktop widths.

