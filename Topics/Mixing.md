
# Mixing Algorithm

The **Machines Position** is defined as the index <br>
of the current container and represented by `x`.

---

## Steps

1. Calculate the distance from `x` to the last element<br>
   when going `clockwise` / `counter-clockwise` .


2. Go along the shorter route.

    *If equal, choose whichever.*


3. Repeat until done.

---

## Calculations

### Delta

Difference to be traversed to the next desired container.

`Δ = Container Index - Position`

### Distance

Distance to be traversed to reach all containers.

`n = Number Of Containers`

##### Counter-Clockwise / Right

`Distance = |Δ|` to the last container.

##### Clockwise / Left

`Distance = |n - Δ|` to the first container.
