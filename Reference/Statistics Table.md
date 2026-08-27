# Statistics Table

*Источник: https://docs.rpg-architect.com/05-reference/statistics-table/*

---

# Statistics Table

## **Statistics Table**[¶](#statistics-table "Permanent link")

A table that maps statistic values to ranks, defining how a character's, class's, or enemy's statistics grow over time.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Growth Statistic

The statistic used to determine growth rate between ranks.

[Statistic](../../06-database/05-statistics/01-statistics/)

Maximum Rank

The highest rank achievable in this table.

Number

Rank Statistic

The statistic that tracks the current rank.

[Statistic](../../06-database/05-statistics/01-statistics/)

Rows

The statistic values at each rank.

[Statistics Row](#statistics-row)

Starting Rank

The initial rank when the table is first applied.

Number

## **Statistics Row**[¶](#statistics-row "Permanent link")

A single row in a statistics table, mapping statistic values to a specific rank.