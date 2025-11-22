[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Don't judge me](https://img.shields.io/badge/Language-Perl_5-steelblue.svg)

# gatherseq

Scan for WGS files and organize them into a JSON file
for transformation into input files for other tools like
Snippy-NG, Bohra, and many others.

## Installation

`gatherseq` has no dependencies except [Perl 5.10](https://www.perl.org/)
or higher. It only uses core modules, so no CPAN needed.

### Direct script download
```
% cd $HOME/.local/bin  # choose a folder in your $PATH
% wget https://raw.githubusercontent.com/tseemann/gatherseq/master/gatherseq
% chmod +x gatherseq
```
### Conda
```
# THIS DOES NOT EXIST YET!
% conda install -c bioconda gatherseq
```
### Github
```
% git clone https://github.com/tseemann/gatherseq.git
% cp gatherseq/gatherseq $HOME/.local/bin # choose a folder in your $PATH
```

## Test Installation

```
% ./gatherseq -v
gatherseq 0.0.4
```

## Examples
```
% gatherseq $HOME/fastq_files/

% gatherseq /home/data/wgs_projects/* > out.json 

```

## Options

* `-M 3` will only traverse 3 folders deep.

## Issues

Submit feedback to the [Issue Tracker](https://github.com/tseemann/gatherseq/issues)

## License

[GPL v3](https://raw.githubusercontent.com/tseemann/gatherseq/master/LICENSE)

## Author

[Torsten Seemann](http://tseemann.github.io/)
