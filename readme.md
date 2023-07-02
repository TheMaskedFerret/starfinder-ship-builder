# Starfinder RPG Ship Builder

A single-page web app for building starships for the Starfinder RPG, by Paizo Inc. This was forked from the original by James Turner. 

## Production and Development Modes

To use Vue.js browser extension (dev mode) add this script towards end of `index.php`:

    <script src="https://unpkg.com/vue"></script>

For production, use:

    <script src="vendor/vue/vue.min.js"></script>

### Dependencies: vue.js and clipboard.js

Set up these files:

    vendor/vue/vue.min.js
    vendor/clipboard/dist/clipboard.min.js

Visit respective vendor sites to get files.

Might also need to copy vendor folder into app.

### Images

SVGs are embedded, so no probs. Might need to copy /img to /app

### File structure

Expected file structure of /app

    /css
    /data
    /img
    /js
    /vendor
    .htaccess
    index.html
    
### Data

A few things to note:

* If building sample ships using the ship builder, output from the ship builder should go in the `params` property in the JSON file. E.g.:

    {
        "id": "inheritorworks-shieldcraft",
        "src": "pact",
        "name": "Inheritorworks Shieldcraft",
        "tier": "8",
        "params": {
            // ship builder output goes here
        }
    }

