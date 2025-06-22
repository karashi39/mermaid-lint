# Rules

## Header Rules

### using 'graph'

**Bad**
```
graph LR
```

**Good**
```
flowchart LR
```

### using 'TD'

**Bad**
```
flowchart TD
```

**Good**
```
flowchart TB
```

## Indent Rules

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
subgraph foo
A --> B
end
```

**Good**
```
subgraph foo
    A --> B
end
```

## Node Rules

### node label not quoted

**Bad**
```
A(label)
```

**Good**
```
A("label")
```

### node label with arrow

**Bad**
```
A --> B("label")
```

**Good**
```
B("label")

A --> B
```

## Arrow Rules

### no space arround arrow

**Bad**
```
A-->B
```

**Good**
```
A --> B
```

### arrow comment not quoted

**Bad**
```
A -->|comment| B
```

**Good**
```
A -->|"comment"| B
```

### chained arrow

**Bad**
```
A --> B --> C
```

**Good**
```
A --> B
B --> C
```

### long arrow

**Bad**
```
A ---> B
```

**Good**
```
A --> B
```

## Style Rules
