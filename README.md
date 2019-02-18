# rust-FileOperator



# rust-FileOperator  (UNDER CONSTRUCTION)

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/RobertBakaric/rust-FileOperator/blob/master/LICENSE)

Rust module for operating with individual text files and/or simplified text database with data are stored in text files in the form of lines separated by " | "

## Installation

To install rust-FileOperator, first install Rust. rust-FileOperator is currently tested on Rust 1.32.0, but it is likely to work on other versions as well.

To install rust-FileOperator itself: 

```
cargo build 
```

## Usage
```

./fo -h


FileOperator 0.1.0
Robert Bakaric <rbakaric@exaltum.eu>

 ________ ________     
|\  _____\\   __  \    
\ \  \__/\ \  \|\  \   
 \ \   __\\ \  \\\  \  
  \ \  \_| \ \  \\\  \ 
   \ \__\   \ \_______\
    \|__|    \|_______|                        
 

USAGE:
    fo [FLAGS] [OPTIONS] --input <FILE> [SUBCOMMAND]

FLAGS:
    -h, --help       Prints help information
    -v               Sets the level of verbosity
    -V, --version    Prints version information

OPTIONS:
    -i, --input <FILE>     Input sam file <required>
    -o, --output <FILE>    Output bam file [default: stdout]

SUBCOMMANDS:
    decrypt    Decrypts the encrypted records
    encrypt    Ecrypts the records
    head       prints first n records
    help       Prints this message or the help of the given subcommand(s)
    select     Selects records depending on the selection key
    split      Selects records depending on the split key
    tail       prints last n records




./fo split   -i in -x ">"|fasta|fastq -n 20|file -o out
./fo head    -i in -x ">"|fasta|fastq -n  20|file -o out
./fo tail    -i in -x ">"|fasta|fastq -n  20|file -o out
./fo select  -i in -x ">"|fasta|fastq -n  20|file -o out
./fo encrypt -i in -x ">"|fasta|fastq -n  20|file -o out
./fo decrypt -i in -x ">"|fasta|fastq -n  20|file -o out
 


```


## License

The software is licensed under the  [MIT license](http://opensource.org/licenses/MIT).

