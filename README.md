This PIMELODUSreadme.txt file was generated on 2021-09-19 by JOSÉ GREGORIO MARTÍNEZ


GENERAL INFORMATION

1. Title of Dataset: Data from: Species limits and introgression in Trans-Andeans Pimelodus from the Magdalena-Cauca River basin

2. Author Information
	A. Principal Investigator Contact Information
		Name: Martínez, José Gregorio
		Institution: Institución Universitaria Colegio Mayor de Antioquia 
		Address: Carrera 78 # 65 - 46 Bloque Patrimonial - Piso 1. Medellín, Antioquia, Colombia
		Email: jose.martinez@colmayor.edu.co

	B. Associate or Co-investigator Contact Information
		Name: Rangel-Medrano, José David
		Institution: Universidad Nacional de Colombia
		Address: Cra. 65 # 59A - 110, Campus el Volador, Medellín, Antioquia, Colombia
		Email: jdrangelm@unal.edu.co
		
		Name: Restrepo-Escobar, Natalia
		Institution: Universidad Nacional de Colombia
		Address: Cra. 65 # 59A - 110, Campus el Volador, Medellín, Antioquia, Colombia
		Email: nrestree@unal.edu.co

		Name: Yepes-Acevedo, Anny Johanna
		Institution: Universidad Nacional de Colombia
		Address: Cra. 65 # 59A - 110, Campus el Volador, Medellín, Antioquia, Colombia
		Email: ajyepesa@unal.edu.co

		Name: Márquez, Edna Judith
		Institution: Universidad Nacional de Colombia
		Address: Cra. 65 # 59A - 110, Campus el Volador, Medellín, Antioquia, Colombia
		Email: ejmarque@unal.edu.co

	
3. Date of data collection: from 2012-01-15 to 2018-12-31

4. Geographic location of data collection: Magdalena-Cauca River Basin, Colombia. Orinoco and Amazon basins from Colombia and Brazil. 

5. Information about funding sources that supported the collection of the data: This research was supported by the scientific cooperation agreement between Universidad Nacional de Colombia, Sede Medellín and Empresas Públicas de Medellín, Grant CT-2019-000661 ‘‘Variabilidad genética de un banco de peces de los sectores medio y bajo del río Cauca’’. This work was further supported by the cooperation of the Institución Universitaria Colegio Mayor de Antioquia (Grant FCS-2017 and FCSA20) and Universidad Nacional de Colombia (Hermes 40096), Grant “Delimitación de Unidades Evolutivas Significativas para la conservación de especies de peces del género Pimelodus en los Andes colombianos: una aproximación genómico-poblacional y filogenómica para la cuenca Magdalena-Cauca” and “Genética de la conservación de especies de peces Trasandinas colombianas del género Pimelodus: una aproximación genómico-poblacional para la cuenca Magdalena-Cauca”. 

6. Recommended citation for this dataset: José Gregorio Martínez, José David Rangel Medrano, Anny Johanna Yepes Acevedo, Natalia Restrepo Escobar, Edna Judith Márquez. Species limits and introgression in Trans-Andeans Pimelodus from the Magdalena-Cauca River basin. Molecular phylogenetics and Evolution.


DATA & FILE OVERVIEW

1. File List: 

Population module parameteres.txt Contains the population module run parameters used on Stacks software v.2.52 and some basic statistics derived. The analysis included genomic RADseqs data Illumina Hi-Seq-derived from 19 individuals of several Pimelodus species.

Demultiplexing statistics.txt Contains the demultiplexing statistics (number os reads by identified barcode) across 19 samples of Pimelodus species libraries obtained by Illumina Hi-Seq, provided by Floragenex Inc. It was included an internal control to compare the efficience of demultiplexing process.

De novo loci assembling statistics.txt Contains the de novo loci assembling statistics (number of loci, number of polymorphic loci and number of SNPs) obtained after the RADproc software analysis across 19 samples of Pimelodus species libraries, using the optimized parameters, by – psweep mode.

Pimelodus.sumstats.summary.txt Contains the summary statistics of variant and fixed positions across loci for each of 19 samples of Pimelodus, after Stacks v.2.52 software analysis (Population module, --fstats).

Pimelodus.var.phylip.txt Contains 999 variable sites for each of 19 samples of Pimelodus in the phylip output encoded using IUPAC notation, using Stacks v.2.52 software (Population module, --phylip-var), suitable for SNAPP and SVDquartets species delimitation analyses. No sites with missing data were inlcuded.

Pimelodus.vcf.txt Contains the output SNPs and haplotypes in Variant Call Format (VCF) for 19 samples of Pimelodus, after Stacks v.2.52 software analysis (Population module, --vcf).

METHODOLOGICAL INFORMATION

1. Description of methods used for collection/generation of data: 
Muscle tissue samples of Pimelodus grosskopfii and P. yuma were collected between 2011 and 2014 and provided by Integral S.A., through two scientific cooperation agreements (19th September 2013; Grant CT-2013-002443). All samples were collected in 18 sites along ~460 km in the mainstream and floodplain lakes of the upper, middle, and lower section of the Colombian Cauca River. In addition, this study also included six samples of P. crypticus from upper section of the Cauca River, properly identified following Villa-Navarro et al. (2017), three samples of P. blochii stricto sensu and P. pictus from Amazon and Orinoco rivers, respectively. Except for two muscle tissues of P. blochii stricto sensu which were provided by the Coleção de Tecidos de Genética Animal (CTGA) of the Laboratório de Evolução e Genética Animal (LEGAL), Federal University of Amazonas, Brazil, samples were bought from local markets and provided by Armando Ortega Lara from the Museo de Ciencias Naturales del Instituto para la Investigación y la Preservación del Patrimonio Cultural y Natural del Valle del Cauca – INCIVA.


2. Methods for processing the data: 
A RAD-seq library was prepared for 19 individuals representing five putative morphospecies of Pimelodus, previously identified by DNA barcoding: three corresponded to P. grosskopfii, P. yuma and P. crypticus from Magdalena-Cauca River basin and two corresponded to the cis-Andean P. blochii stricto sensu and P. pictus. Samples were processed through a single-end sequencing step conducted by Floragenex inc. (http://floragenex.com) on one lane of an Illumina HiSeq 2000 machine. The raw data were de-multiplexed by barcode, quality-filtered, and made a de novo loci construction using RADproc v3 (Nadukkalam Ravindran, Bentzen, Bradbury, & Beiko, 2019) setting up -a psweep mode for the optimization of locus assembling parameters to produce a catalog of RAD-seq tag loci, alleles and SNPs from the raw NGS reads through the different parameter values for m, M and n. Parameters to run RADproc included a Phred Score base quality threshold > 20, a minimum coverage depht of 3 (-m), a maximum distance (in nucleotides) allowed between stacks of 4 (-M), a maximum distance (in nucleotides) allowed between putative loci during catalog construction of 1 (-n), a maximum number stacks per locus of 2 (-x) and minimum sample percentage of 0.9 (-S). Then, we used STACKS v2.53 (Catchen, Hohenlohe, Bassham, Amores, & Cresko, 2013) to generate ouputfiles for population and phylogenomics analyses from the optimal constructed Catalogs obtained by the RADproc analysis. First, we ran in pipeline mode the modules SSTACKS, TSV2BAM, GSTACKS using defaults parameters. Finally we ran the POPULATIONS module following the parameter settings provided in "Population module parameteres.txt". Each individual was considered a population into the STACKS map file. In POPULATIONS module, the minimum number of populations that a locus must be present in to process it, was set to 100% (-p = 19). Likewise, the minimum percentage of individuals in a population required to process a locus for that population was set to 100% (-r = 1) and a minnor allele frequency (MAF) of 0.01. All other parameters for analysis were kept as default. Finally, we obtained VAR.PHYLIP (Pimelodus.var.phylip.txt) and VCF (Pimelodus.vcf.txt) output files containing, respectively, useful dataset for SNPs-based species delimitation and admixture tests. These archives, the summary statistic (Pimelodus.sumstats.summary.tsv.txt)

3. Instrument- or software-specific information needed to interpret the data: 
RADproc v3 (Nadukkalam Ravindran, Bentzen, Bradbury, & Beiko, 2019) and STACKS v2.53 (Catchen, Hohenlohe, Bassham, Amores, & Cresko, 2013). 

