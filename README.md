# POSSUM: a bioinformatics toolkit for generating numerical sequence feature descriptors based on PSSM profiles

![version](https://img.shields.io/badge/version-1.0-brightgreen)
![time](https://img.shields.io/badge/time-15/05/2017-brightgreen.svg)
![Language](https://img.shields.io/badge/python-2.7-blue) 
![Language](https://img.shields.io/badge/language-perl-red) 
![github license](https://img.shields.io/github/license/noHup-cc/POSSUM)
[![Website possum.erc.monash.edu](https://img.shields.io/website-up-down-green-red/http/possum.erc.monash.edu.svg)](http://possum.erc.monash.edu/)
![Unix/Linux](https://svgshare.com/i/Zhy.svg)
![Mac OS](https://svgshare.com/i/ZjP.svg)
![Windows](https://svgshare.com/i/ZhY.svg)



> Authors: [`Jiawei Wang`](http://jiawei.nohup.cc) (chris@nohup.cc) & `Bingjiao Yang` (young@nohup.cc)



## Quick start:

### Prepare running environment

1. Make sure you have installed the following language environments and dependencies.
   - Perl
   - Perl packages
     - Getopt::Long
     - File::Path
     - File::Basename
   - Python 2.7
   - Python 2.7 packages
     - scipy
     - numpy
     - pandas

###  Run the test jobs

1. `unzip/tar POSSUM.zip`

2. `cd POSSUM`

3. `run possum_standalone.pl`

   - For Unix/Linux/Mac OS X users, try any of the following examples:

     ```
     perl possum_standalone.pl -i input/example.fasta -o output/example_aac_pssm.csv -t aac_pssm -p input/pssm_files -h T
     perl possum_standalone.pl -i input/example.fasta -o output/example_smoothed_pssm.csv -t smoothed_pssm -p input/pssm_files -h T -a 7 -b 50
     perl possum_standalone.pl -i input/example.fasta -o output/example_k_separated_bigrams_pssm.csv -t k_separated_bigrams_pssm -p input/pssm_files -h T -a 1
     perl possum_standalone.pl -i input/example.fasta -o output/example_pse_pssm.csv -t pse_pssm -p input/pssm_files -h T -a 1
     perl possum_standalone.pl -i input/example.fasta -o output/example_dp_pssm.csv -t dp_pssm -p input/pssm_files -h T -a 5
     perl possum_standalone.pl -i input/example.fasta -o output/example_pssm_ac.csv -t pssm_ac -p input/pssm_files -h T -a 10
     perl possum_standalone.pl -i input/example.fasta -o output/example_pssm_cc.csv -t pssm_cc -p input/pssm_files -h T -a 10
     ```

   - For Windows users, try any of the following examples:

     ```
     perl possum_standalone.pl -i input/example.fasta -o output/example_aac_pssm.csv -t aac_pssm -p input/pssm_files -h T
     perl possum_standalone.pl -i input/example.fasta -o output/example_smoothed_pssm.csv -t smoothed_pssm -p input/pssm_files -h T -a 7 -b 50
     perl possum_standalone.pl -i input\example.fasta -o output\example_aac_pssm.csv -t aac_pssm -p input\pssm_files -h T
     perl possum_standalone.pl -i input\example.fasta -o output\example_smoothed_pssm.csv -t smoothed_pssm -p input\pssm_files -h T -a 7 -b 50
     perl possum_standalone.pl -i input\\example.fasta -o output\\example_aac_pssm.csv -t aac_pssm -p input\\pssm_files -h T
     perl possum_standalone.pl -i input\\example.fasta -o output\\example_smoothed_pssm.csv -t smoothed_pssm -p input\\pssm_files -h T -a 7 -b 50
     ```

     NOTE: The main usage difference between Windows and other OS is the file path format. POSSUM allows `/`,`\`,`\\` as path separators on windows in accordance with users’ habits.

### Example outputs

1. Two types of input files are needed for POSSUM:
   - `input/example.fasta`: the input fasta file. Users can specify the file path by `-i` parameter.
   - `input/pssm_files`: the folder containing pssm files according to the fasta file. Users can specify the folder path by `-p` parameter.
2. The results of POSSUM are placed in the `output/` folder. Users can specify the folder path and the output file name by `-o` parameter.

### Use POSSUM

1. For detailed usage and description of POSSUM, please refer to [docs/userguide.pdf](docs/userguide.pdf).
2. The POSSUM web server (http://possum.erc.monash.edu/) is available for public access. 
3. Should you have any confusions or suggestions, please email [Dr. Jiawei Wang](mailto:jwang@ebi.ac.uk).

## References

Wang J, Yang B *et al.* POSSUM: a bioinformatics toolkit for generating numerical sequence feature descriptors based on PSSM profiles. *Bioinformatics* 2017;33(17):2756-2758. [DOI: 10.1093/bioinformatics/btx302](https://doi.org/10.1093/bioinformatics/btx302/).
