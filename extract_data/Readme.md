Extracts all game data paks in patch order.

## Example Usage

```
py extract_data.py -d "C:/Games/Steam/steamapps/common/Divinity Original Sin 2" -o "C:/Modding/DOS2DE/Extracted" -l "C:/Modding/DOS2DE/ConverterApp/divine.exe"
```

## Commandline Parameters

| Short Arg  | Long Arg | Description |
| ------------- | ------------- | ------------- |
| -d | --data | The game data directory (where all the game paks are). |
| -o | --output | The output directory to extract all the game data to. |
| -l | --divine | The path to divine.exe ([lslib](https://github.com/Norbyte/lslib/releases/latest)'s commandline tool). |

## Optional Environment Variables

These environment variables will be used as default parameters (so you can omit args like -d and -l).  

| Name  | Description |
| ------------- | ------------- |
| `DOS2_PATH` | The base game directory (such as `Steam/steamapps/common/Divinity Original Sin 2`) |
| `LSLIB_PATH` | The directory that has divine.exe. |

### Adding Environment Variables to Windows 10
In Windows 10 you can add environment variables by:
1. Hit the Windows key, then type `environ`.
2. In the search window click on "Edit the system environment variables."
3. In the new window that opens, click the "Environment Variables" button.
4. Add variables to the "User" side of the pane with the "New" button (use the exact names in the table).

You can refresh environment variables by opening a command prompt and entering `Set PATH=C`, then closing and opening up the command prompt again (to then run the script here in python).

Restarting Windows will reload environment variables as well.