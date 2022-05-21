## Storage Calculation

*In Bytes*

```
+ 1                                # Recipe Count

for recipe in recipes:

    + 1                            # Name Length
    + X  Recipe -> Name -> Length  # ASCII Characters

    + 1                            # Spices Count

    for spice in spices:

        + 1                        # Spice Position
        + 1                        # Spice Amount
```
