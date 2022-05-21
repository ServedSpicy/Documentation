
# Config Parsing

When requested, the **WebServer** will <br>
load / parse the data contained in the <br>
`Recipes.yaml` / `Spices.yaml` configs.

## Returned Data

The response to these requests is met with <br>
not only the parsed data but also any known <br>
**Error** that occurred while parsing.

This allows the client to give the user choices <br>
over **How** / **If** the data should be used when it <br>
contains errors.

## Recipe Errors

In the following a list of possible parsing <br>
errors for the recipe config is listed:

| Error | Description |
|:-----:|:------------|
| `FailedToReadFile` | The file doesn't exist, is protected,..
| `CouldntParseYAML` | The config contains a **YAML** syntax error.
| `NoDataAvailable` | The config file is empty.
| `WrongStructure` | The root object isn't an object / table / map.
| `MissingRecipeData` | The recipe doesn't contain any data.
| `RecipeDataIsntObject` | The recipe data isn't an object / table / map.
| `NameTooLong` | The recipes name is longer than `20` characters.
| `RecipeUsageNotBoolean` | A recipes `Used` property lists a non-boolean value.
| `RecipeSpicesNotObject` | A recipes spices data isn't an object / table / map.
| `RecipeSpiceAmountNotNumber` | A spices amount isn't a number.
| `RecipeSpiceAmountNotInteger` | A spices amount isn't an integer;
