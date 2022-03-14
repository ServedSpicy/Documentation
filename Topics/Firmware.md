
# Firmware

## Process

#### Power On

```
    [ Power On ]
         🡇
     [ Setup ]
         🡇
 [ Draw Main Menu ]
         🡇
⟳ [ Idle / Check ]
↳ [   Serial Available ? ]    🡆  [ Start Synchronization ]
↳ [ Any Button Pressed ? ]  🡆  [ Start Navigation ]

```

#### Synchronization

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
        [ Idle ]
```

#### Navigation

```

```