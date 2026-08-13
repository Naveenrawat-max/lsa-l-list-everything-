# lsa (List everything)
I have made this tool as an alternative to the `ls -l` command on Linux. This script loops through the directory you run it against and lists all the files and everything that your directory contains. It will be shown hierarchically and color-coded.

This tool will show content like this:

```
/path/to/directory
Subdirectories and contents:
   ├── file1.txt
└── sub_dir
       ├── executable_file
    └── sub_sub_dir
           ├── file3.txt
```

*   **Directories** are shown in blue.
*   **Executables** are shown in green.
*   **Regular files** are shown in the default terminal color.

### Installation

[-] To run this script just clone this repo to your machine. Check the permissions; if it is not executable, give it executable permission:
```bash
chmod +x lsa
```
[-] You can move it to your `/usr/local/bin` directory to make it globally available:
```bash
sudo mv lsa /usr/local/bin/
```

### Usage

[-] Run it in your current directory:
```bash
lsa
```

[-] Or, pass a specific directory path to list its contents:
```bash
lsa /path/to/your/directory
```
