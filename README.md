# dsl-experiment
Basic implementation of Hindley-Milner Type System and variants.

Suggested reading: [Compositional Type Checking for Hindley-Milner Type Systems with Ad-hoc Polymorphism](https://gergo.erdi.hu/projects/tandoori/Tandoori-Compositional-Typeclass.pdf)

### compile
```
stack setup
stack build
```

### run

load module in GHCi then run `test` function

```
stack ghci Compositional.hs
stack ghci Curry.hs
stack ghci MilnerMycroft.hs
stack ghci HindleyMilner.hs
```

i.e. run `test` of `MilnerMycroft`

```
stack ghci MilnerMycroft.hs

[1 of 1] Compiling MilnerMycroft
Ok, modules loaded: MilnerMycroft.

*MilnerMycroft> test
```


try `Compositional` with parser:

```
stack ghci ParseTrifecta.hs

[1 of 2] Compiling Compositional
[2 of 2] Compiling ParseTrifecta
Ok, modules loaded: Compositional, ParseTrifecta.

*ParseTrifecta> test'
```
