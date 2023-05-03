# Gitignore Cheatsheet

The `.gitignore` file is used to specify files and directories that should be ignored by Git. This is useful when sharing your code with others, as there are often files or parts of your project that you do not want to share. Here are some examples of patterns that can be used in `.gitignore` files:

## Matching files

* To ignore a single file, add its name to the `.gitignore` file:
    ```
    example.txt
    ```

* To ignore all files with a certain extension, add the extension preceded by a `*`:
    ```
    *.log
    ```

* To ignore all files with a certain name, add the name preceded by a `/`:
    ```
    /build/
    ```

* To ignore all files in a certain directory and its subdirectories, add the directory name followed by a `/`:
    ```
    logs/
    ```

* To ignore a specific file in a directory and its subdirectories, add the file path to the `.gitignore` file:
    ```
    /logs/example.log
    ```

## Matching directories

* To ignore a directory and its contents, add the directory name to the `.gitignore` file:
    ```
    build/
    ```

* To ignore a specific subdirectory within a directory, add the subdirectory name to the `.gitignore` file:
    ```
    build/temp/
    ```

* To ignore a directory that has already been committed to Git, use the `git rm` command:
    ```
    git rm -r --cached build/
    ```

## Matching patterns

* To ignore files based on a pattern, use a regular expression:
    ```
    *.log
    *.tmp
    ```

* To ignore all files in a directory and its subdirectories based on a pattern, use a regular expression:
    ```
    logs/**/*.log
    ```

These are just a few examples of the patterns that can be used in `.gitignore` files. For more information, refer to the Git documentation on [.gitignore files](https://git-scm.com/docs/gitignore).
