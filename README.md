# Examples for the Quantum ESPRESSO (QE) app

Collection of examples of core app features ready to be imported in the QE app.

## How to add new examples

To add a new example, place the corresping AiiDA archive file (.aiida) in the `core` folder and add an entry in the `core/metadata.json` fill in the following format:

```json

[
    ...,
    {
        "name": "<name of the file>",
        "label": "<a short label to be used in an example selector>",
        "description": "<short description of what the user can expect from the example>",
    }
]
```

## Versioning

This repo will be tagged to mark its compatability with versions of the QE app.

### Rules

- Modifying the structure of the repo requires a new tag
- Updating existing examples requires a new tag
- Adding new examples does not require a new tag - instead, update the tag to the commit of the new example(s)
