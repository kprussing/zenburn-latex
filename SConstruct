#!/usr/bin/env python

import os

env = Environment(TEXINPUTS=os.curdir,
                  tools=["default", "dtxtools"] )

root = "zenburn-latex"
pdf = env.PDF(root + ".dtx",
              MAKEINDEX=env["MAKEINDEX"] + " -s gind.ist")
stys = env.ins2sty([], root + ".ins")
Depends(pdf, stys)
if not GetOption("clean"):
    Default(pdf)

slides = env.PDF("example-slides.tex")
Depends(slides, [str(x) for x in stys if "theme" in str(x)])

