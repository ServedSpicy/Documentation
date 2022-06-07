
# Mixing Algorithm

The **Machines Position** is defined as the index <br>
of the current container and represented by `x`.

<br>
<br>

## Steps

1. Calculate the distance from `x` to the last element<br>
   when going `clockwise` / `anti-clockwise` .


2. Go along the shorter route.

    *If equal, choose whichever.*


3. Repeat until done.

<br>

---

<br>

## Calculations

### Delta

*Distance to the next container.*

`Δ = Container Index - Position`

<br>

### Distance

*Total distance to traverse to reach all containers.*

`n = Number Of Containers`

<br>

##### ⭯  /  Right

*Distance to the last container.*

`Distance = |Δ|`

<br>

##### ⭮  /  Left

*Distance to the first container.*

`Distance = |n - Δ|`

<br>
