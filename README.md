# Ubiquinone-prediction
------
## Required tools
------
> * BLAST+


## Configuration Tool
----------------------
Download and Install BLAST+

**Step 1:**	We used the version "ncbi-blast-2.9.0+", download BLAST+ from:

        ftp://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/
  

**Step 2:** Install the BLAST+ by following the  user manual, you can find the user manual from:  

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
       
**Step 4:**  Combine the Step 3's features into 820-dimensional features

**Step 5:** Select the top 242-dimensional features according to the ranking results of feature importance

**Step 6:** Load the model adjusted by the Particle swarm optimization algorithm

**Step 7:** Predict whether the current protein is UBP

**Step 7:** Get conclusion

## Model flowchart
![image](https://github.com/JiangWenJie-stack/Ubiquinone-prediction/blob/master/images/flow%20chart.png)
