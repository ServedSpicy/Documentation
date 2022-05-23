
# Firmware

<br>

## Process

#### Power On

```
  [ Power On ]
       🡇
   [ Setup ]
       🡇
[ Recipes Menu ]
```

#### Recipes Menu

```
         🡇
  [ Read Recipes ]
         🡇
[ Draw Recipes List ]
         🡇
⟳ [ Idle / Check ]
↳ [   Serial Available ? ]  🡆  [ Synchronize ]
↳ [ Any Button Pressed ? ]  🡆  [ Navigate ]

```

#### Synchronize

```
[ Start Synchronization ]
           🡇
⟳ [ Wait For 2 Bytes ]      # Amount of bytes to write
           🡇
⟳ [ 0 ➞ Amount ]
↳ [ Wait For Byte ]
↳ [     Read Byte ]         # Serial
↳ [    Write Byte ]         # EEPROM
           🡇
   [ Recipes Menu ]
```

#### Navigate

```
↳ [   Right   ] 🡆 [ Mixing Menu ]
↳ [ Up / Down ] 🡆 [ Check / Update Index ]
                              🡇
                       [ Recipes Menu ]
```

#### Mixing Menu
