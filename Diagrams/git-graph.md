---
lang: en-US
title: GitGraph 
---


## GitGraph Diagram

```mermaidjs
gitGraph
    commit
    branch develop
    commit tag:"v1.0.0"
    commit
    checkout main
    commit type: HIGHLIGHT
    commit
    merge develop
    commit
    branch featureA
    commit
```
