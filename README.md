# RevilToolset-AutoBatch

An updated version of my standalone Revil batch tool that works with SaladSoftware. It's as easy as going to the new tab in the GUI and telling the program where your files are. The only con is that, for now, you have to download RevilToolset yourself before you can use it.

There are two paths you can take in using this program:

1. Include .arc extraction and mod + lmt -> gltf in one go (I recommend doing this)
2. The old-fashioned method of extracting the arc *then* running the script. You don't have to do it this way, but if you already have a bunch of extracted files that you want consolidated into gltf then go for it!

The output will go into a new folder where your chosen input is.

I have only tested this program on Windows. If it doesn't work for you, then please do report any issues. My environment shouldn't be so specific that something would work for me but not for you, but I can't guarantee that.

(Building also might be broken right now... I would recommend just installing the dependencies and running SaladSoftware.py to be safe)

Happy modding!

## Features

- **MT: Revil Conversion Tab**: A new tab in SaladSoftware's UI to use the tool.
- **Automatic Unpacking**: Extracts `.arc` archives using integrated MT logic.
- **Smart Pairing**: Automatically matches animation files (`.lmt`) to models (`.mod`) by name.
- **Recursive Scan**: Process entire folders and subfolders in one go.
- **Batch Processing**: Handles multiple conversions with progress tracking and logging.
- **Cleanup**: Automatically removes temporary `batch.json` files after successful conversion.

## Requirements

- **Python 3.8+**
- **RevilToolset**: This *must* be installed somewhere on your computer, how else are you gonna use it?
- **Python Dependencies**:

  ```bash
  pip install pycryptodome tkinterdnd2 tqdm
  ```

## Usage

Run the main application:

```bash
python SaladSoftware.py
```

Navigate to the **MT: Revil Conversion** tab, select your assets folder and the path to your RevilToolset utilities, and click **Start Revil Conversion**.
