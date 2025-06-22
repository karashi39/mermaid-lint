# Rules


### useless indent

**Bad**
```
flowchart LR

    A --> B
```

**Good**
```
flowchart LR

A --> B
```

### no indent in subgraph

**Bad**
```
subgraph
A --> B
end
```

**Good**
```
subgraph
    A --> B
end
```

