Reflect on This

1. Getting Help:
    Linux has `man`, `--help`, and `help` because they serve different purposes: 
    -> `man` gives detailed manual pages, `--help` provides quick usage info for external commands, and `help` explains shell built-ins.  
        This separation ensures accurate, context-specific help depending on the command type.  

    Scenario:
    -> `help` is the only correct choice when seeking information about a **shell built-in** (e.g., `cd`),  
        because built-ins have no separate executable to run with `--help` and may lack detailed `man` pages.

2. Searching Files:
    The key difference is that:
    -> `ls | grep ".txt"` lists files in the **current directory only** and filters them by name pattern.  
    -> `find . -name "*.txt"` searches **recursively** through the current directory and all subdirectories.

    More powerful:  
    -> `find` is more powerful when you need to search deep into folder structures, apply conditions (e.g., by size, date).

3. Piping to grep:
    -> history | grep keyword
       [ eg: history | grep docker ]

4. Archiving:
    why send .tar.gz instead of .zip to linux user:
    -> Preserves Linux permissions and metadata better than .zip.
    -> Is a native, commonly used Linux format and often compresses better.

    Security Risk:
    -> An archive from an unknown source could contain malicious files or scripts that overwrite important system files or run harmful code.  
       Always inspect its contents before extracting and only extract in a safe, isolated directory.
