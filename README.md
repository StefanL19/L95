# L95

This directory contains the parses produced by the RASP System and the Charniak Parser on the sentences contained in the 
dataset.txt file.

The file charniak_input.txt contains the input to the Charniak Parser.

The file charniak_trees_output.txt contains the output of the Charniak Parser in the form of trees. The output in the form of
SD (Stanford Dependencies) may be found in pdf format in the detailed output directory, where the name of each subdirectory
corresponds to the id of the sentence mentioned in dataset.txt file

The file rasp_input.txt contains the input to the RASP System.

The file rasp_grs_output.txt contains the output of the RASP System in the form of GRs.

The directory conll_files/ is structred in the following way
* charniak.conll contains the output of the Charniak Parser in the of form of SD which were converted to be compatible with
the CONLL-X format.
* rasp.conll contains the output of the RASP System in the form of GRs which were converted to be compatible with the CONLL-X
format.
* gt_gr.conll ground truth annotation which follows the GRs scheme and are used for measuring the performance of the RASP System
* gt_stanford ground truth annotation which follows the SD scheme and are used for measuring the performance of the Charniak
Parser

The directory detailed_output/ is structured in the following way
* The names of the subdirectories correspond to the names of ids of the sentences in the dataset.txt file
* Additional preprocessing steps like manually supplying PoS tags corresponding to each one of the sentences is 
located in those folders.
* The pdf files contain the SD outputs of the Charniak Parser
