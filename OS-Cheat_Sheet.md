---

### 🧾 Python `os` Module Cheat Sheet

| **Function**                          | **Description**                                                                 | **Example**                                  |
|--------------------------------------|---------------------------------------------------------------------------------|----------------------------------------------|
| `os.getcwd()`                        | Returns the current working directory                                           | `cwd = os.getcwd()`                          |
| `os.chdir(path)`                     | Changes the current working directory                                           | `os.chdir('/home/user/folder')`              |
| `os.listdir(path='.')`               | Lists files and directories in the specified path                               | `files = os.listdir()`                       |
| `os.mkdir(path)`                     | Creates a single directory                                                      | `os.mkdir('new_folder')`                     |
| `os.makedirs(path)`                  | Creates directory and all intermediate-level directories                        | `os.makedirs('folder/subfolder')`            |
| `os.rmdir(path)`                     | Removes an **empty** directory                                                  | `os.rmdir('empty_folder')`                   |
| `os.removedirs(path)`                | Removes directories recursively                                                 | `os.removedirs('folder/subfolder')`          |
| `os.remove(path)`                    | Deletes a file                                                                  | `os.remove('file.txt')`                      |
| `os.rename(src, dst)`                | Renames a file or directory                                                     | `os.rename('old.txt', 'new.txt')`            |
| `os.path.exists(path)`               | Checks if a path exists                                                         | `os.path.exists('file.txt')`                 |
| `os.path.isfile(path)`              | Checks if a path is a file                                                      | `os.path.isfile('file.txt')`                 |
| `os.path.isdir(path)`               | Checks if a path is a directory                                                 | `os.path.isdir('folder')`                    |
| `os.path.getsize(path)`             | Returns file size in bytes                                                      | `size = os.path.getsize('file.txt')`         |
| `os.path.getmtime(path)`            | Returns last modified time as a **Unix timestamp**                              | `ts = os.path.getmtime('file.txt')`          |
| `os.path.abspath(path)`             | Returns the absolute path                                                       | `abs_path = os.path.abspath('file.txt')`     |
| `os.path.join(path1, path2, ...)`   | Joins paths using the correct separator for the OS                             | `os.path.join('folder', 'file.txt')`         |
| `os.environ`                         | Accesses environment variables                                                  | `os.environ['HOME']`                         |
| `os.environ.get(key)`               | Gets the value of an environment variable                                       | `os.environ.get('PATH')`                     |
| `os.system(command)`                 | Executes a shell command (use `subprocess` instead for new code)               | `os.system('ls -l')`                          |
| `os.name`                            | Returns the name of the OS-dependent module imported (`'posix'`, `'nt'`, etc.) | `print(os.name)`                             |

---

### 🧠 Handy Extras:
- Use `datetime.fromtimestamp(ts)` (from `datetime` module) to convert Unix timestamps into human-readable dates.
- Prefer `os.path.join()` over manual slashes to ensure cross-platform compatibility.
- Use `os.path` submodule for most path-related operations.

---

Let me know if you want this as a downloadable file or converted into flashcards or something interactive!