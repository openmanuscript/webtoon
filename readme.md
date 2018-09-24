## tools for web comics

A set of simple tools for web comics. The tools support the following workflow:

- Draw line art on paper, then scan into an image.
- use `dtoon --scantoline` to convert the scanned image into line art.
- incorporate the resulting image into final colored art (with a tool of your
  choice. Save that out as final artwork.
- use `dtoon --shrink` to convert the final artwork into the final resolution
  you need.

The script assumes that the current date is used to name and organize the files.
It creates a directory with the current date, and names the files according to
the following convention. The second number in the name is the step of the
workflow, so that files appear in the order they are used.

```
    2018-09-22/
        2018-09-22_01-scan.png
        2018-09-22_02-line.png          (created by --scantoline)
        2018-09-22_03-final.png
        2018-09-22_04-final_800px.png   (created by --shrink)
```
