# doicheck
These are Nushell scripts designed to retrieve IDs from common citation databases. To ensure full functionality, you'll need API keys for both Web of Science and Scopus. By default, the scripts expect your keys to be stored in `~/.config/doicheck/config.json`.

The script `doicheckdatase` is specifically created to help augment data exported from the Swedish digital repository DiVA (*Digitala Vetenskapliga Arkivet*), though it can likely be repurposed for your own use cases. This script takes two arguments: the first is the CSV file you want to augment, and the second is the name for the new augmented file. You can choose the output format as CSV, JSON, or TSV depending on the file ending in the argument you provide, with CSV as the default.

The `doicheck` script takes one argument—a DOI—and searches Web of Science, Scopus, and PubMed, displaying the found identifiers in the terminal.

## Dependencies
`nushell` (tested on version 0.104.1)

