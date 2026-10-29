# Kit Launcher

A one-page static site that turns an ordinary https link into an app link, so a row in Notion can open a model kit in DEVONthink or Obsidian.

- `https://rh-stevens.github.io/kit-launcher/#dt-<DEVONthink group UUID>` — opens the kit's group in DEVONthink (`x-devonthink-item://`)
- `…/#ob-<UUID>` — opens the kit's note in Obsidian (`obsidian://open?vault=my_obsidian_Vault&file=Model Tracker/Kits/<note>`)
- `…/#<UUID>` — shows both buttons
- no hash — searchable list of all kits

The kit map (`const KITS` in `index.html`) is generated from the Obsidian `Model Tracker/Kits` notes by the model-database skill. Regenerate and commit when kits are added.
