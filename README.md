# mdfmt

mdfmt automatically reformat Markdown files with some heuristic rules.  

Usually, I run it once for one or more Markdown files and then manually fix the rest of warnings.

1. Run mdfmt with all Markdown files in a directory

   ```bash
   mdfmt *.md
   ```
   
1. Alternatively run the following two steps until no more lint errors.

   1. Run [`markdownlint-cli`](https://github.com/igorshubovych/markdownlint-cli).
   
      ```bash
      markdownlint -c .markdownlint.yaml *.md | sort
      ```
      
   1. Manually fix lint errors.
