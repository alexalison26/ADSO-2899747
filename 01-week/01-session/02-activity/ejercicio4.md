  ┌─────────────────────┐
          │     Rama Feature     │
          │  (feature/HU-xxxx)   │
          └─────────┬───────────┘
                    │
                    ▼  MR a Dev
          ┌─────────────────────┐
          │        DEV           │
          │ Desarrollo y pruebas │
          └─────────┬───────────┘
                    │
                    ▼  MR a QA
          ┌─────────────────────┐
          │         QA           │
          │ Pruebas de calidad   │
          └─────────┬───────────┘
                    │
                    ▼  MR a Main
          ┌─────────────────────┐
          │        MAIN          │
          │ Producción estable   │
          └─────────────────────┘
1.Se crea una rama desde dev o main para trabajar en una HU.

2.Se hace un MR a dev para integrar el cambio y probarlo en desarrollo.

3.Si pasa en dev, se hace un MR a qa para pruebas de calidad.

4.Si pasa en qa, se hace un MR a main para producción.

5.Opcional: Si es un proyecto grande con varios módulos, antes de qa se puede integrar en una rama project.

