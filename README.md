# Vialgo

> Note: Vialgo is in an early stage.

Vialgo is a web app for writing and visualizing algorithms.

[dev.to](https://dev.to/aldober)

# Idea

- The user will select one of the pre-generated templates (Array, Grid, Tree, etc..) and will be directed to the "Editor".

- The "Editor" will have two sections, one for the user to write the program and the other to visualize the output.

- the program will be written in "Vialgo-Lang", a proprietary scripting syntax.

# Example - Bubble Sort algorithm written in vialgo-lang
```
type array

function setup()
    set(random_ints(0, 100, 10))
end

function main()
    n = length()
    loop i in series(n - 1)
        loop j in series(n - 1)
            i1 = get(j)
            i2 = get(j + 1)

            if i1 > i2
                swap(j, j + 1)
            end
        end
    end
end
```
