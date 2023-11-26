## Repro

```markdown
> * Foo
> * Bar
```

> * Foo
> * Bar

Can you see "Foo" or "Bar"? Try advancing the slide.


## Explicit `nonincremental` class restores expected behavior {.smaller}

```markdown
> :::{.nonincremental}
> * Foo
> * Bar
> :::
```

> :::{.nonincremental}
> * Foo
> * Bar
> :::

I wasn't able to find anything in the docs about this implicit incremental behavior.


## Doesn't repro with paragraph text in quote


```markdown
> This text restores expected behavior
>
> * Foo
> * Bar
```

> This text restores expected behavior
>
> * Foo
> * Bar


## Multiple lists are even weirder

```markdown
* Foo
* Bar

> * Baz
> * Qux
```

* Foo
* Bar

> * Baz
> * Qux

Can you see "Baz" or "Qux"? Try advancing the slide.
