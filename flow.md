# What is this?

A flowchart [using Mermaid support in Markdown files](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) (h/t/ to [Lewis](https://github.com/asos-lewisjackson) for the pointer)

```mermaid
flowchart TD
  A[Deploy to production] --> B{Is it Friday?};
  B -- Yes --> C[Do not deploy!];
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
Establish community         :done,    des1, 2021-09-01,2021-10-01
Define working group        :done,    des2, 2021-09-01,2021-12-01
Produce pilot               :done,    des3, 2021-10-01,2021-12-01
Sign off pilot              :done,    des4, after des2,2022-01-01
Plan schedule               :         des5, after des4, 2022-03-01
Source equipment and tools  :         des6, after des4, 2022-03-01
```

