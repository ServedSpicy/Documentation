
# EEPROM

Recipes with spices resolved to their container number.

Available Memory on **Arduino UNO** : `1024B`

## Recipe Resolving

Using the container configuration tuples `< Position | Spice >`, <br>
one can resolve a recipes ingredient lists keys from being names <br>
to the more compact position of the spice container.

This way we also don't have to upload the container configuration itself.

## Structure

```
     Ｂｙｔｅ
[  Recipe Count ]

        Ｂｙｔｅ      Ｂｙｔｅ[]          Ｂｙｔｅ          Ｂｙｔｅ     Ｂｙｔｅ
[ ( { Name Length } { Chars } ) ( { Spices Count } { [ Position ] [ Amount ] } { ... } { ... } ) ]
[ ... ]
[ ... ]
```

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
