[Blog](https://medium.com/@utkarshvijay99/docker-optimizations-9bbd3ea7e658)
The reason for copying the `package.json` and `package-lock.json` files separately from the `src` directory is to take advantage of Docker's layer caching. If the `package.json` and `package-lock.json` files haven't changed since the last build, Docker can reuse the cached layer for those files, which can significantly speed up the build process. If the `package.json` and `package-lock.json` files were in the same directory as the `src` directory, Docker would have to copy all of those files every time, even if the `src` directory hasn't changed.

## metadata 
Metadata is additional data that provides information about the main data or object.

- **For a Book:**
  - Metadata can include details such as the author's name, publisher, publication date, genre, ISBN, and more. These pieces of information help identify and categorise the book, making it easier to organize and search for.

- **For a Website:**
  - Metadata in the context of a website includes elements like meta tags in HTML, which can include keywords, descriptions, and other information. This metadata aids in search engine optimisation (SEO) by providing additional context to search engines about the content of the website.
## Archive file

Archive files are used to collect multiple data files together into a single file for easier portability.
compose of one or more files in one single file along with metadata
## tar
so tar basically combines every file in one archive file called tarball for distribution or backup processes. name comes from "tape archive" as it was used for i/o devices which doesn't had any os and used magnetic tapes.


## POSIX
(portable operating system interface)
POSIX standards define file-related functions like `open()`, `read()`, `write()`, and `close()`

## Egg vs .Whl

When you install a package in .egg format:
the system download a tarball (tar file)
then system builds a .whl file (which is nothing but a compiled zip of all dependencies)
then system installs the actual packages from whl file (wheel)
downloading and compiling the tar file makes whole process time-consuming

wheel modules are better than egg because they allow python modules to be installed without requiring a build process. This means that users can simply download a wheel package and install it using the pip command, without needing to compile the package from the source code or install any additional dependencies.

### FIX
Whenever you get error where dependecy is not fetched using apt-get try to clear cache by using docker prune command