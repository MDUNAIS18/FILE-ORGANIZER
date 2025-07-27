File Organizer Automation Script:
This Python script automatically organizes files in a selected folder into subfolders based on file types such as Images, Documents, Videos, Audio, Archives, and more. It also logs each file movement and error into a log file for easy tracking.

Features:
 * Automatically scans and organizes files into categorized folders
 * Supports various file types: images, documents, audio, video, archives, and code files
 * Unrecognized files are moved into an "Others" folder
 * Automatically creates folders if they do not exist
 * Generates a detailed log file (organizer_log.txt) with timestamps
 * Handles errors gracefully with logging and exception handling

File Type Categories:
 * Images: .jpg, .jpeg, .png, .gif, .bmp
 * Documents: .pdf, .docx, .txt, .xlsx, .pptx
 * Audio: .mp3, .wav, .m4a
 * Videos: .mp4, .mkv, .flv, .avi
 * Archives: .zip, .rar, .tar, .gz
 * Scripts: .py, .js, .java, .cpp
 * Others go to an Others folder.

How It Works:
  * Set the target folder path where your unorganized files are located.
  * The script checks all files in that folder.
  * Each file is moved to a corresponding folder based on its extension.
  * A organizer_log.txt file is created to track the operation.
    
Setup Instructions:
1. Clone the Repository or Copy the Script:
  bash
  Copy
  Edit
  git clone https://github.com/yourusername/file-organizer.git
  cd file-organizer
  Or just copy the .py script into your working directory.

2. Modify Folder Path:
In the script, change this line to point to your target folder:

  python
  Copy
  Edit
  source_folder = r"E:\INFOTACT SOLUTION"
Or uncomment the input line to take user input dynamically:

  python
  Copy
  Edit
  file_location_path = input("Enter the folder path to organize files: ").strip()
 
 3. Run the Script
  bash
  Copy
  Edit
  python file_organizer.py
  After execution, check your folder. Files will be moved into their respective subfolders, and the log will be available at organizer_log.txt.

 Requirements: 
  * Python 3.12.8
  * No third-party packages required (uses only built-in modules: os, shutil, logging)

Sample Folder Structure (After Organizing):
  mathematica
  Copy
  Edit
  E:\INFOTACT SOLUTION\
  │
  ├── Images\
  ├── Documents\
  ├── Audio\
  ├── Videos\
  ├── Archives\
  ├── Scripts\
  ├── Others\
  └── organizer_log.txt
