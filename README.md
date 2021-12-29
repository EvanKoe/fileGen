# NP - a program that generates sample files for you

This program is a shortcut to create new projects. It copies your main files to the directory of your choice, using a given extension (sh, c, cpp).

# Installation

```bash
git clone https://github.com/EvanKoe/np.git && cd np
```
Then, create a link in your path to use it everywhere :  
```bash
sudo ln np /usr/bin
```
Then edit the `np` file and replace the `PATH` variable with the directory that contains your np file :
```
10 | PATH = "~/Documents/Tek2/lib"  <-- replace with your np directory (without any final '/')
```

# Usage
To get help, juste type `np -h`. It will display :  
```bash
np -t TYPE -d DIR -n NAME
```
Where :  
- `TYPE` is your file type (`sh`, `c` or `cpp`),
- `DIR` is the destination directory
- `NAME` is the name of your destination file (optional)

For example, the line  
```bash
np -t sh -d . -n test
```
will copy a simple executable program called `test.sh` into the `.` directory. 

# Customization

You can customize the file Np copies. To achieve this, do simply edit one of the sample files in the repo you just cloned (`main.c`, `main.cpp` or `main.sh`). In a next update, I'll add the capacity to clone multiple files (a file.c and header.h for example) at once.

# License
Use this file as you wish. Make it better if you can, just enjoy the FOSS ideology :)
