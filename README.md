# To Create a Custom Folder Icon

1. To create a custom folder icon you will need a two files with one of the files ending in `-open`. For example
    - folder-sample.svg
    - folder-sample-open.svg
2. Place the icons in a folder under `~/.vscode/extensions`
3. Next open your vscode settings.json and add
    ```
    "material-icon-theme.folders.associations": {
        "src": "../../../../NEW_ICON_FOLDER_NAME_HERE/ICON_FILE_NAME_HERE"
    }
    ```
    Replacing `NEW_ICON_FOLDER_NAME_HERE` and `ICON_FILE_NAME_HERE` with their respective names. Also change the `src` to the be name of the folder you want the icon to apply to
    <br>It should end up like this
    ```
    "material-icon-theme.folders.associations": {
        "iam": "../../../../icons/folder-iam"
    },
    ```
    
    > **Note**
    > If you want to use an existing icon provided by `Material Icon Theme`. It should look like `../../../icons/folder-xxx`


4. Restart Vscode and your new Icon should appear!
