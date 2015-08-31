# Virus Identification Pipeline (VIP)

VIP-0.1.0 Quick Start Guide & National Institute for Viral Disease Control and Prevention

VIP performs the following steps to achieve its goal: (i) map and filter out background-related reads, (ii) extensive classification of reads on the basis of nucleotide and remote amino acid homology, (iii) multiple k-mer based de novo assembly and phylogenetic analysis to provide evolutionary insight.

There results of VIP were displayed in HTML format. A demo result was available at http://yang.hukaa.com/1/

# Introduction

Virus Identification Pipeline (VIP) is a one-touch computational pipeline for virus identification and discovery from metagenomic NGS data, rigorously tested across multiple clinical sample types representing a variety of infectious diseases. VIP has been tested on Ubuntu 14.04 and Biolinux 8. Other Linux distribution would be supported but not tested.

# Installation

The steps to install VIP on a machine are as follows:

1.	Install all dependencies (run db_installer.sh and dependancy_installer.sh )
2.	Decompress VIP.tar.gz, make sure all the files can be executed.
3.	Generating the config file, details as following.
4.	Run VIP

# Config files

The config file includes parameters for VIP to run. Each parameter can be modified based on your situation. Generally the default parameters are suitable for most cases.

# Usage

	Create default config file.
		VIP.sh -z -i <NGSfile> -p <454/iontor/illumina> -f <fastq/fasta/bam/sam> -r <reference_path>

	Run VIP with the config file:
		VIP.sh -c <configfile> -i <NGSfile>

	Run VIP with verification mode
		VIP.sh -i <NGSfile> -v

# Helps

Any questions can be sent to liyang@ivdc.chinacdc.cn


