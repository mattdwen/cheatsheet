# Cheatsheet

## Code

- **C# Pattern Matching**

  ```c#
  public void HandleException(Exception ex) {
    if (ex is MyCustomException customEx) {
      // Do thing with the custom type
    } else {
      // Do thing with a normal exception
    }
  }
  ```

## Editors

Atom, Visual Studio, and VS Code.

- **Find in Files**

  `ctrl+shift+f`

- **Markdown Preview**

  `ctrl+shift+m`

  *Note: Custom binding in VS Code.*

## Git

- **Force Push**

  ```
  git push origin master --force
  ```

- **Rebase**

  ```
  git checkout experiment
  git rebase master
  ```

## PowerShell

- **List the size of sub folders**

  ```
  Get-ChildItem | Where-Object { $_.PSIsContainer } | ForEach-Object { $_.Name + ": " + "{0:N2}" -f ((Get-ChildItem $_ -Recurse | Measure-Object Length -Sum -ErrorAction SilentlyContinue).Sum / 1MB) + " MB" }
  ```

- **Tail**

  ```
  Get-Content .\path\to\file.txt -wait
  ```

## Visual Studio

- **Search Solution Explorer**

  `ctrl+;`
