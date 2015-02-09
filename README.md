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


