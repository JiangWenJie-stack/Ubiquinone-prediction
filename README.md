# Ubiquinone-prediction
------
## Required tools
------
> * BLAST+
> * Swissprot


## Configuration Tool
----------------------
Download and Install BLAST+

**Step 1:**	We used the version "ncbi-blast-2.9.0+",download BLAST+ from:

        ftp://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/
  

**Step 2:** Install the BLAST+ by following the  user manual, you canfind the user manual from:  

         https://www.ncbi.nlm.nih.gov/books/NBK1762/

**Step 3:** We used the swissprot data set. release the data set to the relative paths ./blast/db/ ,download the data set from:

        ftp://ftp.ncbi.nlm.nih.gov/blast/db/
        

**Step 4:** Change the path of BLAST+ in the "RunBlast.py"				".../blast/"

## Configuration Tool
---------------
**Step 1:**	Input the ID of the protein

**Step 2:**	Crawl fasta files from:

                https://www.uniprot.org/

**Step 3:**	  
>>>3.1 Get 20-dimensional amino acid composition 

       CalculateAAC(self,ProteinAdderss):

>>>3.2 Get 400-dimensional dipeptide composition

       CalculateDipeptideComposition(self,ProteinAdderss):

>>>3.4 Get 400-dimensional standardized PSSM

       standed_PSSM(self,SimplifyPssm(self,pssmdir,ID),ProteinAdderss):
       


## Model flowchart
![image](https://github.com/JiangWenJie-stack/Ubiquinone-prediction/blob/master/images/flow%20chart.png)
