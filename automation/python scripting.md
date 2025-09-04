### hashbang
python shell scripts start with a very specific line

```
#! /usr/bin/env python3 -> called a hashbang

#! -> tells the system to use /usr/bin/env python3 to run the file

/usr/bin/env python3 -> means to search in this path for python3 and use it 

```

### why env instead of python3 or other paths?
on [[linux]] python may have different locations like `/bin/python3` or `/usr/bin/python3`, using **env** searches in your [[PATH]], for python and uses the first one it finds

so using **env** makes the script more portable

*without the hashbang you would need to launch the script with `python3 script.py`*

### permissions 
every scripts needs to be made into an executable using [[chmod]]

```
chmod +x script.py
```

# common libraries for python scripting
- [[os-lib]] -> environments, file paths, permissions
- [[subprocess-lib]] -> run commands
- [[shutil-lib]] -> copy/move/remove files
- [[pathlib]] -> modern path handling
- [[argparse-lib]] -> parse command-line arguments