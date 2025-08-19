# Google Drive Shared Folder Copy

This Google Colab notebook copies the full content of a **shared Google Drive folder** into your own Google Drive account, preserving the folder structure.

---

## Features

- Pulls files recursively, preserving folders inside your Drive.
- Simple, customizable destination folder setting.
- Shows file copy progress with filename and size.
- Handles Google Drive API authentication automatically on Colab.

---

## Usage

1. Open the `copy-gdrive-folder.ipynb` notebook in [Google Colab](https://colab.research.google.com).
2. Edit the cell with the two configuration variables:

    ```
    SRC_FOLDER_URL = "https://drive.google.com/drive/folders/your-shared-folder-id"
    DEST_PATH = "/YourDriveFolder/SubFolder"
    ```

3. Run all cells.  
4. The script will copy files to `MyDrive/YourDriveFolder/SubFolder`.  
5. Check the output log for number of files copied and any errors.

---

## Requirements

- Run inside Google Colab (because it mounts Google Drive and uses the Drive API).  
- Shared Google Drive folder URL must be accessible ("Anyone with the link" permission).

---

