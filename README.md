About Chisel
============

Chisel is an open-source hardware construction language developed
at UC Berkeley that supports advanced hardware design using highly
parameterized generators and layered domain-specific hardware languages.

Chisel is embedded in the [Scala](http://www.scala-lang.org/) programming
language, which raises the level of hardware design abstraction by providing
concepts including object orientation, functional programming, parameterized
types, and type inference.

Chisel can generate a high-speed C++-based cycle-accurate software simulator,
or low-level Verilog designed to pass on to standard ASIC or FPGA tools
for synthesis and place and route.

Visit the [community website](http://chisel.eecs.berkeley.edu/) for more
information.

This repo contains chisel documentation. Code is kept in a separate repo.

Documentation
-------------

In order to generate the Chisel documentation (html and pdf formats),
you'll need the LaTeX tools, tex4ht, texlive, python bs4
BeautifulSoup, imagemagick, and source-highlight.

To generate all the documentation:

    $ make

### Dependencies
The following
apt-get installs should work for ubuntu 14.04 LTS

    $ sudo apt-get install python-bs4 python-jinja2 imagemagick source-highlight
    $ sudo apt-get install tex4ht texlive-latex-base
    $ sudo apt-get install texlive-latex-recommended texlive-latex-extra
    $ sudo apt-get install texlive-fonts-recommended texlive-fonts-extra
    
On Mac OsX first install [MacTeX](https://tug.org/mactex/mactex-download.html) then use brew 

    $ brew install miktex
    $ brew install imagemagick source-highlight
    $ brew install gawk

and then downaload Beautiful Soup from [site](http://www.crummy.com/software/BeautifulSoup/#Download) unpack and run inside the folder

    $  python setup.py install
