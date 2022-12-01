# Jancy Example Resolver Plug-in

## Structure of the Plug-in
- `example-preloadaer/package.json` - A simple file that describes the plugin to Jancy and specifies an entry point. `src/index.js` in this example.
- `example-preloader/src/index.js` - This is the main file that implements most of our plugins logic. The most important part is the object exported that has a couple of very specific jancy properties and functions (jancy_props, jancy_onInit, jancy_onEnabled, jancy_onDisabled). That's probably where you should start.

## Adding the Plug-in to Jancy

1. Open the Jancy plug-in folder
    - On Windows, open Windows File Explorer and go to %appdata%\Jancy\plugins or on MacOS
    - On MacOS, open Finder and go to `TODO`
2. Copy `example-preloader` folder to the plug-ins folder from step 1.
3. Restart Jancy if it's already running.
4. If everything works correctly you should see the example plugin in the list of plugins in `File -> Settings -> Plugins`.
5. In any tab in Jancy go to `stubhub.com` and you should see a button in the upper left corner that the example plugin added.
6. In another tab, go to the URL `jancy://example`
7. Every time you press the button in the stubhub tab, you'll see the counter increment in the example page.
