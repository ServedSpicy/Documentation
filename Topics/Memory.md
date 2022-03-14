

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

<br>

---

<br>

## Controller EEPROM Memory

Recipes with spices resolved to their container number.

Available Memory on **Arduino UNO** : `1024B`

### Recipe Resolving

Using the container configuration tuples `< Position | Spice >`, <br>
one can resolve a recipes ingredient lists keys from being names <br>
to the more compact position of the spice container.

This way we also don't have to upload the container configuration itself.

### Structure

```
         byte         byte[]            byte             byte        byte
[ ( { Name Length } { Chars } ) ( { Spices Count } { [ Position ] [ Amount ] } { ... } { ... } ) ]
[ ... ]
[ ... ]
```

### Storage Calculation

*In Bytes*

```
for recipe in recipes:
    + 1                         # Name Length
    + recipe -> name -> length  # ASCII Characters
    + 1                         # Spices Count
    
    for spice in spices:
        + 1                     # Spice Position
        + 1                     # Spice Amount    
```


