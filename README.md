# Examples for the Quantum ESPRESSO (QE) app

Collection of examples of core app features ready to be imported in the QE app.

## How to add new examples

To add a new example, place the AiiDA archive file (.aiida) in the `archives` folder and add a corresponding entry in the `examples.json` file in the following format:

```
{
    ...,
    "<archive_name.aiida>": {
        "label": "<a short label to be used in an example selector>",
        "description": "<short description of what the user can expect from the example>",
    }
}
```

#### Metadata format

Using the archive filename `"<archive_name.aiida>"` as key simplifies metadata lookup, for example, displaying an example description on user selection.

## Versioning

This repo will be tagged to mark its compatability with versions of the QE app.

#### Rules

- Modifying the structure of the repo requires a new tag
- Updating existing examples requires a new tag
- Adding new examples does not require a new tag - instead, update the tag to the commit of the new example(s)
