# Data Tables Reference — UX Movement Corpus

## Table Fundamentals

### Visual Hierarchy in Tables
- Not all columns are equally important; reflect this visually
- Primary identifier column: bold or slightly larger
- Secondary data: regular weight, lighter color
- Status badges: use color + label
- "10 Design Tips for a Better Data Table Interface"
- "UI Design Tips for a Better Data Table UX"

### Row Density
- Tight: 32–36px row height (data-dense apps, power users)
- Comfortable: 48px (general apps)
- Spacious: 56–64px (when rows contain multi-line or image content)

### Column Headers
- Left-align text columns; right-align numeric columns
- Sortable headers: show sort icon (hidden until hover for secondary columns)
- Fixed header on scroll for long tables

## Filters

### Filter placement
- Filters belong inside or directly above the table header
- Panel-based filters (sidebar or overlay) are slower — more distance between controls and data
- "How to Design the Best Table Filters" + Part 2
- "Why Data Table Filters Work Better in Headers"
- "The Right Way to Design Custom Table Filters"
- "The Best Filter UI Design for Large-Scale Apps"
- "How to Simplify 20 Dropdown Filters Without Removing Any"

### Filter patterns for large option sets (>100 options)
- Searchable filter dropdown
- Group options into categories
- "How to Handle a Massive Filter with Over 100 Options"
- "The Best UX Design for a Long List of Filters"

### Multi-select filters
- Use multiselect menus (not checkboxes in a list)
- "Start Using Multiselect Menus for Your Filters"
- "Stop Using Listboxes for Multiselecting Items"

### Filter state visibility
- Show active filters as chips below the table header
- Include "clear all" control
- Show result count update in real time

## Sorting

- Primary sort: single click on column header
- Don't use dropdown menus for sorting — column click is faster
- "Why You Shouldn't Use Dropdown Menus for Data Sorting"
- "How to Simplify the Most Complex Data Sort"

## Bulk Actions

- Hide bulk action toolbar until at least one row is selected
- Show selected count in toolbar
- Confirm destructive bulk actions
- "A Better UX Approach to Faster Table Bulk Actions"
- "The Best Bulk Edit UI for Data Tables"
- "The Easiest Way to Bulk Edit Data Tables"

## Row Actions

- Reveal action buttons on row hover
- For dense tables: use icon buttons with tooltips (not text labels)
- "How to Fit 8 Action Buttons in a Table Row"

## Status Badges

- Use semantic colors + text labels (never color alone)
- Active/success → green; pending/warning → yellow; error/inactive → red/gray
- "The Right Way to Design Table Status Badges"

## Comparing Rows

- Sticky selected row or row highlighting
- Side-by-side comparison panel for detail view
- "A Better UI to Bulk Compare Table Rows Faster"
- "How to Make Cluttered Content Cards Easier to Compare"

## Wide Tables with Many Columns

- Freeze important columns (identifier, status)
- Allow column reordering and hiding
- "How to Simplify a Massive 19 Column Data Table"
- "The Easiest Way to Condense Wide Data Tables"

## Data Visualization in Tables

- Sparklines, mini bars, and color scales add context to numeric columns
- "How to Make Your Data Tables More Visual"
- "Data Cards Make Table Numbers Easier to Read"
- "How to Turn Data Lists into Interactive Charts"
- "Why You Should Turn Raw Data Lists into Rich Interactive Charts"

## Mobile Tables

**Anti-pattern**: horizontal scroll for wide tables on mobile
**Solutions**:
- Stacked list (card per row, key fields visible)
- Priority column display (hide secondary columns)
- Responsive column collapsing

- "The Best Mobile Layout for Complex Data Tables"
- "How to Make Data Tables Look Great on Mobile"
- "How to Display Large Data Tables on Small Screens"
- "Stacked List: The Best Way to Fit Tables on Mobile Screens"

## Pagination

- "View More" button > numbered pagination for most content
- Numbered pagination: good when users need to return to specific pages
- Show total count and current range
- "How to Display a Pagination of 100 Data Rows"
- "Why View More Buttons Are Better Than Pagination Links"

## Empty States

- Show a helpful message + CTA when the table is empty
- Don't leave a blank white space

## Data Cards (Alternative to Tables)

- For numeric dashboards: cards scan faster than table rows
- Include trend indicator, change %, and comparison period
- "Data Cards Make Table Numbers Easier to Read"
- "Why Data Cards Are Faster to Scan Than Tables"
- "A More Efficient Way to Display Data Tables"
