Extracts all game data paks in patch order.

# Usage

```
py extract_data.py -d "G:/Divinity Original Sin 2/DefEd/Data" -o "D:/Modding/DOS2DE/Extracted" -l "G:/Modding/DOS2DE/ConverterApp/divine.exe"
```

## Commandline Parameters

| Short Arg  | Long Arg | Description |
| ------------- | ------------- | ------------- |
| -d | --data | The game data directory (where all the game paks are). |
| -o | --output | The output directory to extract all the game data to. |
| -l | --divine | The path to divine.exe ([lslib](https://github.com/Norbyte/lslib/releases/latest)'s commandline tool). |

## Optional Environmental Variables

These environmental variables will be used as default parameters (so you can omit args like -d and -l).

| Name  | Description |
| ------------- | ------------- |
| DOS2_PATH | The base game directory (such as `Steam\steamapps\common\Divinity Original Sin 2`) |
| LSLIB_PATH | The directory that has divine.exe. |
