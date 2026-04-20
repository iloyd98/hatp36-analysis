# HAT-P-36 Analysis

This project has two notebooks:
- spectrum_pipeline.ipynb
- transit_pipeline.ipynb

---

## STEP 1: Download everything

1. Download this repo.
2. Open the Google Drive link:

https://drive.google.com/drive/folders/1fTodVuM6U_5bwtF_rLCyS34d3GN17Qdi?usp=sharing

3. Inside the Google Drive folder, you will see two folders:
   - FAST
   - KeplerCam

Download BOTH folders.

Note: KeplerCam is a large download and may take some time. Also, due to the large file size, the KeplerCam data will be zipped into 3 separate files. More on this below.

---

## STEP 2: (IMPORTANT) Fix the folder names

Google Drive WILL rename folders when downloading. KeplerCam will download in multiple folders (more on this below).

Make sure the folders are named EXACTLY:

FAST  
KeplerCam, KeplerCam1, KeplerCam2  

They may download as something like:
- FAST-20260419T023638Z-3-001  

Rename them before continuing.

---

## STEP 3: Extract the zip files

Each download will be a .zip file.

Extract all zip files.

IMPORTANT (KeplerCam only):

1. Unzip all 3 KeplerCam files.
2. Open Terminal.
3. Navigate to the folder containing KeplerCam, KeplerCam1, KeplerCam2 (cd /Users/YOURNAME/...)
4. Run:
   rsync -av KeplerCam*/ KeplerCam/

5. Verify there are 619 files in KeplerCam by copying and pasting this into terminal and pressing enter:
   
   find KeplerCam -type f | wc -l

   If the output says 619, then you did this part correctly!

---

## STEP 4: Move the folders

Drag and drop (or copy/paste) BOTH KeplerCam and FAST folders into the data folder.

---

## STEP 5: Run the notebooks

Open the notebook folder.

Open each notebook and run ALL cells:

1. spectrum_pipeline.ipynb
2. transit_pipeline.ipynb

---

## NOTES

- Do NOT change any file paths!
- Everything should run as-is.
- All plots will appear in the notebook.
