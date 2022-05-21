
# EEPROM

*Persistent Data On The Machine.*

<br>

## Size

The current setup uses the **Arduino UNO**. <br>
⤷  `1024 Bytes`

<br>
<br>

## What

*A list of things that are saved on the EEPROM.*

| Name | From | Size | Description |
|:----:|:----:|:----:|:------------|
| ***Recipes***      | `0`    | `1000` | Resolved recipe data |
| ***EERPOM Guard*** | `1023` | `1`    | Remedies looping when EEPROM is corrupted

<br>
<br>

## Data

### Recipes

*Resolved recipe data with <kbd>Recipe Name</kbd> ,* <br>
<kbd>Container Position</kbd> *&* <kbd>Spice Amount</kbd>

<br>
<br>

<div align = center>

![Recipe Data]

</div>

<br>
<br>

#### Sizes

| Component | Bytes | Description |
|:---------:|:-----:|:------------|
| ***Recipe Count*** | `1` | The count of recipes following
| ***Name Length***  | `1` | Char count of name, not null terminated
| ***Spice Count**   | `1` | Count of position - amount pairs
| ***Position***     | `1` | Position of the spices container
| ***Amount***       | `1` | Relative amount of spice to be mixed









<!--   🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶  🌶   -->

[Recipe Data]: ../Resources/Firmware/Recipe%20Data.svg
