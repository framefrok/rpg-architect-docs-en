# Statistics Table Editor

*Источник: https://docs.rpg-architect.com/04-editor/statistics-table-editor/*

---

# Statistics Table Editor

## **Statistics Table Editor**[¶](#statistics-table-editor "Permanent link")

The Statistics Table Editor is where a statistic's value at every rank is authored. It is the same editor everywhere it appears — [Characters](../../06-database/00-characters/00-characters/), [Classes](../../06-database/00-characters/01-classes/), [Enemies](../../06-database/06-enemies/00-enemies/), [Equipment](../../06-database/02-items/02-equipment/), and [Skills](../../06-database/01-skills/01-skills/) all use it.

The editor works in two formats, switched with the Table / Graph toggle. **Table** lists one row per rank and is what you edit directly. **Graph** plots the same values as a curve, which is the faster way to judge whether growth accelerates or flattens where you intended.

Rank and Growth choose which statistic drives progression and which one measures it, and Minimum and Maximum Rank set how far the table extends. Export, Import, and Reset act on the whole table at once.

The values the table holds are documented under [Statistics Table](../../05-reference/statistics-table/).

![The Statistics Table Editor in Table format, with one row per rank](../media/img_34_statistics-table.png)

### ![1](../media/img_17_marker-01.png) Rank Statistic[¶](#rank-statistic "Permanent link")

The statistic that tracks the current rank - the column the table is keyed on.

### ![2](../media/img_18_marker-02.png) Growth Statistic[¶](#growth-statistic "Permanent link")

The statistic that accumulates toward the next rank. In a level-based setup this is experience.

### ![3](../media/img_20_marker-03.png) Rank Range[¶](#rank-range "Permanent link")

The lowest and highest rank the table covers. Widening the range adds rows; narrowing it drops them.

### ![4](../media/img_22_marker-04.png) Export / Import / Reset[¶](#export-import-reset "Permanent link")

Moves the whole table in and out of a file. Tables this large are usually easier to author in a spreadsheet and import back.

### ![5](../media/img_23_marker-05.png) Table / Graph[¶](#table-graph "Permanent link")

Switches between editing the raw numbers and seeing them plotted, which makes an uneven growth curve obvious at a glance.

### ![6](../media/img_28_marker-06.png) Values[¶](#values "Permanent link")

One row per rank and one column per statistic in Table mode; one editable curve per statistic in Graph mode. The calculator opens a **Formula editor** from a column header in Table mode, and a **Curve editor** from a card in Graph mode. In Graph mode you can also click a point on a curve to set that rank's value directly.

![The formula editor opened from a column header, listing the constants, functions and statistic names an expression can use](../media/img_35_statistics-formula.png)

### ![1](../media/img_17_marker-01.png) Formula[¶](#formula "Permanent link")

The expression evaluated for every rank in the column, written in the engine's own formula syntax. The names listed under **Variables** below are the other statistics, so one column can be derived from another.

### ![2](../media/img_18_marker-02.png) Initial Value[¶](#initial-value "Permanent link")

The value the first rank starts from, where the formula needs somewhere to begin. Both boxes expand into a larger editor with the arrow at their right.

## **Graph Mode**[¶](#graph-mode "Permanent link")

![The Statistics Table Editor in Graph mode, plotting each statistic's curve across its rank range](../media/img_36_statistics-graphs.png)

![The curve editor opened from a graph card, generating a statistic's values from an easing function with optional random variance](../media/img_37_statistics-curve-editor.png)

### ![1](../media/img_17_marker-01.png) Easing / Formula[¶](#easing-formula "Permanent link")

How the curve is generated - stepped through an easing function, or evaluated from a formula.

### ![2](../media/img_18_marker-02.png) Easing Function[¶](#easing-function "Permanent link")

Which easing function shapes the curve, and whether it runs in reverse. See [Easing Function Editor](../easing-function-editor/).

### ![3](../media/img_20_marker-03.png) Start / End Values[¶](#start-end-values "Permanent link")

The range the curve spans - the value at the first rank and the value at the last.

### ![4](../media/img_22_marker-04.png) Random Variance[¶](#random-variance "Permanent link")

How far each rank's value may drift from the curve, so growth need not be perfectly smooth.

### ![5](../media/img_23_marker-05.png) Current / Preview[¶](#current-preview "Permanent link")

The values the table holds now, beside the ones these settings would produce.