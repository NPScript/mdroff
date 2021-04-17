# MDRoff

Convert *markdown* to *roff*.

If you use `eqn` you can use the *math*-context:

```  math
psi~''~left ( x right ) + { 8 cdot pi sup 2 cdot m } over h sup 2 cdot E cdot psi~left ( x right ) = 0
```

## How to get a PDF

Just pipe the output of `mdroff` to `groff`.

``` sh
# Use the '-e' flag if your using 'eqn'
mdroff your_file.md | groff -ms -e -k -Tpdf > output.pdf
```
