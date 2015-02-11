*Update*: this low-memory bug has been [fixed](https://github.com/chrchang/plink-ng/commit/a3b34a675f0482b89d7acb9fc4ea8fedf87f3d45).


Setup
-----

Download and build tool binaries. Assumes 64-bit linux platform.

```bash
$ make install-tools
```

Install Python packages (numpy, pandas, matplotlib). One way:

```bash
$ pip install -r requirements.txt
```

Analysis pipeline
-----------------

```bash
$ make init fetch-vcf
```

```bash
$ make FMT=bin project
```

![64-bit float](publish/ldmatrix.10000.bin.2015-02-08.png)

```bash
$ make FMT=bin4 project
```

![32-bit float](publish/ldmatrix.10000.bin4.2015-02-08.png)


Result using plink-1.07 `--matrix` with 5kb bins:

![plink1](publish/plink1.5000.bin4.2015-02-09.png)
