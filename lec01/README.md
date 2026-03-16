What version is your samtools command in the bioinfo environment?

```bash

$ micromamba list | grep samtools
  samtools                   1.23          h96c455f_0            bioconda   
(bioinfo) 

```


Show commands needed to create a nested directory structure.

```bash

$ mkdir -p dir1/dir2/dir3

$ tree dir1
dir1
`-- dir2
    `-- dir3

3 directories, 0 files

```

Show commands that create files in different directories

```bash

$ touch ./dir1/dir1file | ls dir1
dir1file  dir2

```

Show how to use relative and absolute paths.

```bash
ABSOLUTE PATH
$ ls /home/kennethdungca/Documents/Bioinformatics/tests-only/dir1/
dir1file  dir2

RELATIVE PATH
$ ls dir1/
dir1file  dir2
```
