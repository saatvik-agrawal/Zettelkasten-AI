## manifest.json



  /* id is not finalised as I need to ensure its unique */
  /* main.js will be generated from main.ts using npm run build.  */



## versions.json

{
  "0.1.0": "0.15.0"
}
🧠 What This Means
"0.1.0" = your plugin's current version
"0.15.0" = the minimum Obsidian version required to run it
As you update your plugin:

Add new entries (e.g. "0.2.0": "0.16.0")
Older Obsidian versions will automatically get the most compatible plugin version
