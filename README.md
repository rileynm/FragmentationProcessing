# FragmentationProcessing
A set of tools for processing Byonic search results to inspect fragmentation and identification quality.

Input the Byonic .csv outputs into GlycoDataScanAssigner_Batch. Also needed are .raw files.
Use list.txt files from GlycoDataScanAssigner_Batch as input for the GlycoFragmentFind_Batch_ver2, in addition to .raw files and a Uniprot database file that contains all glycosites annotated in the proteome (downloadable from the Uniprot website). .
Use the list.txt files from GlycoDataScanAssigner_Batch, the scoredSpectra.txt files, a Uniprot database file that contains all glycosites annotated in the proteome (downloadable from the Uniprot website), and the N- and O-glycan databases used in the Byonic searches as input for GlycoCompiler_Batch. Users can input score filters, deltaMod cutoffs, sites allowed per glycopeptide, logProb cutoffs, peptide length cutoffs, and FDR cutoffs.
GlycoCompiler_Batch outputs 7 files for each .raw file/Byonic result: dataSummary file, Glycans, GlycoPepties, GlycoProteins, GlycoPSMs, GlycoSites, and GlycoUniqSeq. GlycoPSMs is the most useful file for evaluating spectral quality.
