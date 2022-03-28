

## User Config Files

Data used for the GUI configuration interface.

### Recipes

Format: `YAML`

##### Template

```yaml
<Recipe Name>:
    Used : <Is Used>
    Spices:
        <Spice A> : <Amount>
        <Spice B> : <Amount>
```

##### Example

```yaml
Cicken Mix:
    Used : true
    Spices:
        Oregano : 4
        Garlic : 8
        Red Pepper : 6
```

<br>

### Spices

Format: `YAML`

```yaml
- <Spice A>
-
- <Spice B>
```

##### Example

```yaml
- Oregano
- Garlic
-
-
- Red Pepper
-
```
