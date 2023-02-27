# PowerBI CheatSheet

## Ranking based on Cumulative GPA(Rank column)

```sh
Rank = RANKX(all('Sheet_Name'), [Cumulative GPA],,DESC)
```

## Creating a column which says yes for the top 20% or top 1/5th students, else No

```sh
Top 1/5th = IF([Rank] <= DIVIDE(COUNT(‘Sheet_Name’[Cumulative GPA]), 100) * 20,"Yes","No")
```
