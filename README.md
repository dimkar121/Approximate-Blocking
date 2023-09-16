# Approximate Blocking
This is the artifact for the manuscript:

"A Suite of Efficient Randomized Algorithms for Streaming Record Linkage", 

co-authored by D. Karapiperis (IHU), C. Tjortjis (IHU), and V. Verykios (HOU).


## Abstract
Organizations leverage massive volumes of information and new types of data to generate unprecedented insights and improve their outcomes. 
Correctly identifying duplicate records that represent the same entity, such as user, customer, patient and so on, a process commonly known as record linkage, can improve service levels, accelerate sales, or elevate healthcare decision support. 
Towards this direction, blocking methods are used with the aim to group matching records in the same block using a combination of their attributes as blocking keys. 
This paper introduces a suite of randomized algorithms specifically crafted for streaming record linkage settings. Using a bounded in-memory data structure, in terms of the number of blocks and positions within each block, 
our algorithms guarantee that the most frequently accessed and the most recently used blocks remain in main memory and, additionally, the records within a block are renewed on a rolling basis. 
The operation of our algorithms rely on simple random choices, instead of utilizing cumbersome sorting data structures, 
which ensure that the probability of inactive blocks and older records to remain in main memory decays in order to free space for more promising blocks and fresher records, respectively. 
We also introduce an algorithm that performs approximate blocking to tackle the problem of misspellings and typos present in the blocking keys. 
The experimental evaluation showcases that our proposed algorithms scale efficiently to data streams by providing certain accuracy guarantees.


## Running the artifact
The source has been tested with Python version 3.8
- Clone the repo
- The `requirements.txt` file lists all Python modules that the source file `SCD.py` depends on. These modules can be installed using:
  `pip3 install -r requirements.txt`.
