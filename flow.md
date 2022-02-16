# What is this?

A flowchart [using Mermaid support in Markdown files](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) (h/t/ to [Lewis](https://github.com/asos-lewisjackson) for the pointer)

```mermaid
flowchart TD
  A[Deploy to production] --> B{Is it Friday?};
  B -- Yes --> C[Run deploy.sh to deploy! We have robust systems and Friday is just another day!];
  B -- No --> D[Run deploy.sh to deploy!];
  C ----> E[Enjoy your weekend];
  D ----> E[Enjoy your weekend];
```

## Gantt

```mermaid
gantt
dateFormat  YYYY-MM-DD
title ASOS Tech Podcast 🎙
excludes weekdays 

section M1 Discovery 
Establish community         :done,    dis1, 2021-09-01, 2021-10-01
Define working group        :done,    dis2, 2021-09-01, 2021-12-01
Produce pilot               :done,    dis3, 2021-10-01, 2021-12-01
Sign off pilot              :done,    dis4, after dis2, 2022-01-01
Plan schedule               :active,  dis5, after dis4, 2022-03-01
Source equipment and tools  :active,  dis6, after dis4, 2022-03-01

section M2 Season 1 
Produce Tech Ep 1&2        :    first1, 2022-02-24, 2022-03-25
Produce DITLO Ep 1&2       :    first2, 2022-03-03, 2022-03-25
Sign off first 4 eps       :    first3, after first2, 10d
Define ASOS Tech brand     :    first4, 2022-01-01, 2022-03-18
Build podcast website      :    first5, after first4, 2022-03-25
Sign off podcast website   :    first6, after first5, 10d
Release Ep 1               :    first7, after first6, 14d
Release Ep 2               :    first8, after first7, 14d
Release Ep 3               :    first9, after first8, 14d
Release Ep 4               :    first10, after first9, 14d
Produce Tech Ep 3&4        :    first11, 2022-04-07, 14d
Produce DITLO Ep 3&4       :    first12, 2022-04-21, 14d
Sign off first 4 eps       :    first13, after first10, 10d
Release Ep 5               :    first14, after first13, 14d
Release Ep 6               :    first15, after first14, 14d
Release Ep 7               :    first16, after first15, 14d
Release Ep 8               :    first17, after first16, 14d

```

