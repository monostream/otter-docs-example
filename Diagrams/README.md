---
lang: en-US
title: Diagrams
---

# MermaidJS Integration

Otter Docs integrates with [MermaidJS](https://mermaid-js.github.io/mermaid/#/) 

Checkout [Mermaid.Live](https://mermaid.live/) to create stylish diagrams like:


## Otter reproduction!

```mermaid
    graph TD 
        A[Male Otter] --> B[Femal Otter] 
        B --> C[Child Otter 01] 
        B --> D[Child Otter 02]
```

## Otter lifestyle

```mermaid
graph TD
    A[Hungry] -->|catch fish| B(Eat)
    B --> C{What next?}
    C -->|One| D[more fish]
    C -->|Two| E[wank]
    C -->|Three| F[fa:fa-otter reproduce]
```


## One otter after the otter


```mermaid
sequenceDiagram
  BabyOtter->PapaOtter: Hello Hello, how hungry are you?
  loop Every minute
    BabyOtter-->PapaOtter: nomnom fishy fishy!
  end
```


## Otter class diagram

```mermaid
classDiagram
    Animal <|-- Otter
    Animal <|-- Fish
    Animal <|-- Duck
    Otter <|-- Omni_Otter
    Fish <|-- Omni_Otter
    Duck <|-- Omni_Otter
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
      +String beakColor
      +swim()
      +quack()
    }
    class Fish{
      -int sizeInFeet
      -canEat()
    }
    class Otter{
      +bool is_wild
      +run()
    }

    class Omni_Otter{
      +bool is_crazy
      +bool has_multi_inhertiance
      +run()
    }

```


## OTTER ER-DIAGRAMS

```mermaid
erDiagram
          OTTER }|..|{ MOUTH : has
          OTTER ||--o{ FISH : catches
          OTTER ||--o{ INSTINCT : "liable for"
          MOUTH ||--o{ FISH : receives
          INSTINCT ||--|{ FISH : covers
          FISH ||--|{ MEAT : includes
          HUNGER ||--|{ MEAT : contains
          HUNGER ||--|{ INSTINCT : contains
          
```


## Otter Journey

```mermaid
  journey
    title No idea what this diagram is used for
    section Happy day
      Wake up: 5: Otter
      Go swim: 8: Otter
      Releax: 1: Otter
      Eat: 10: Otter, Cat
    section Go home
      Go swim: 5: Cat
      Eat fish: 3: Otter, Cat
```

## Otter git graph

```mermaid
    gitGraph
      commit
      commit
      branch develop
      checkout develop
      commit
      branch feature-otter
      checkout feature-otter
      commit
      commit
      commit
      checkout main
      merge feature-otter
      merge develop
      commit
      commit
```

