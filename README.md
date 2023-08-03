# pyEager

A simple package to read in eager results.

## Available functions

 - `compile_endogenous_table()`: Creates a compiled table of endogenous DNA statistics from endorspy including all the information in the list of JSON file paths provided. Wraps `parse_endorspy_json` on all provided JSON paths.
    - `parse_endorspy_json()`: Read in the information in a single endorspy JSON file.
 - `compile_damage_table()`: Creates a compiled table of select DamageProfiler results from the list of JSON files provided. Ths resulting dataframe includes the number of reads analysed by DamageProfiler as well as the damage in the first 2 bp of either end of DNA molecules for each sample.
    - `collect_damageprofiler_results()`: Collects the results from multiple damageprofiler JSON output files into a large dictionary containing all the results for each sample. This function wraps `parse_damageprofiler_json` across all provided JSON files.
    - `parse_damageprofiler_json()`: Read in the information in a single damageprofiler JSON output file. 
 - `compile_snp_coverage_table()`: Creates a compiled table of SNP coverage results from the list of JSON files provided. Wraps `parse_snp_coverage_json` across all provided JSON files
    - `parse_snp_coverage_json()`: Read in the information in a single SNP coverage JSON file.
 - `parse_sexdeterrmine_json()`: Reads in the Sexdeterrmine output JSON into a dataframe.
 - `parse_nuclear_contamination_json()`: Reads in the nuclear contamination output JSON into a dataframe.
 - `parse_eager_tsv()`: Reads in the eager input TSV into a dataframe.
 - `parse_general_stats_table`: Reads in the general stats table output of MultiQC into a dataframe.

## Installation

<!-- TODO Add installation instructions -->

## Usage

<!-- TODO Add usage examples -->

## License

[MIT](LICENSE.txt)