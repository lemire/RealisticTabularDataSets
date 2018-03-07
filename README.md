# RealisticTabularDataSets
Some realistic tabular datasets for testing (CSV)

The datasets are gzipped, you can unzip them under Linux and macOS with the gunzip program. Windows users can use [7-Zip](http://www.7-zip.org). Mac users should be able to just double-click on the files to uncompress them.

These data sets have been used in several academic papers.


## Census-Income

File: census-income.data.gz 5.7MB

Census-Income is a relatively small data set with 100 MB and 199 523 records. However, it has 42 columns and one column has a very high relative cardinality (99 800 distinct values). 

We include a subset (census-income.data.d241850.csv.gz) made of 4 columns: age, wage per hour, dividends from stocks and a numerical value found in the 25th position of the original data set. The respective cardinalities are 91, 1 240, 1 478 and 99 800.

Source:

* Frank, A. and Asuncion, A. 2010. UCI machine learning repository. http://archive.ics.uci.edu/ml

## Census 1881

File: census1881.csv.gz 33MB

Census 1881 comes from the Canadian census of 1881: it has over 4 million records. Census1881 came from a publicly available SPSS file 1881 sept2008 SPSS.rar that we converted to a flat file. In the process, we replaced the special values “ditto” and “do.” by the repeated value, and we deleted all commas within values. The column cardinalities are 183, 2 127, 2 795, 8 837, 24 278, 152 365, 152882.

Source: 

* Lemire D, Kaser O, Gutarra E. [Reordering rows for better compression: Beyond the lexicographical order](https://arxiv.org/abs/1207.2189). ACM Transactions on Database Systems 2012; 37(3), doi:10.1145/2338626.2338633.

## Weather

File: weather_sept_85.csv.gz 15MB

It consists of  surface synoptic weather reports from land stations for September 1985. 

Source:

* Frank, A. and Asuncion, A. 2010. UCI machine learning repository. http://archive.ics.uci.edu/ml
*  Hahn, C., Warren, S., and London, J. 2004. Edited synoptic cloud reports from ships and land stations over the globe, 1982–1991. http://cdiac.ornl.gov/ftp/ndp026b/


## Wikileaks

File: wikileaks-noquotes.csv.gz 5.9MB

The Wikileaks table was created from a public repository published by Google and it contains the non-classified metadata related to leaked diplomatic cables. We extracted 4 columns: year, time, place and descriptive code. It has 1 178 559 records. Our Wikileaks table has column cardinalities 273, 1440, 3935 and 4865.

Source: 

* Lemire D, Kaser O, Gutarra E. [Reordering rows for better compression: Beyond the lexicographical order](https://arxiv.org/abs/1207.2189). ACM Transactions on Database Systems 2012; 37(3), doi:10.1145/2338626.2338633. 


## Sorted versions

File: census-income_srt.csv.gz

File: wikileaks-noquotes_srt.csv.gz

File: weather_sept_85_srt.csv.gz

File: census1881_srt.csv.gz

We sorted the tables lexicographically, with the smallest cardinality column being the primary sort key, the next-smallest cardinality column being the secondary sort key, and so forth.

References:  

* Lemire, D., Kaser, O., Kurz, N., Deri, L., O'Hara, C., Saint‐Jacques, F. and Ssi‐Yan‐Kai, G., 2017. [Roaring bitmaps: Implementation of an optimized software library](https://arxiv.org/abs/1709.07821). Software: Practice and Experience 48 (4), 2018.
* Lemire, D., Ssi‐Yan‐Kai, G. and Kaser, O., 2016. [Consistently faster and smaller compressed bitmaps with roaring](https://arxiv.org/abs/1603.06549). Software: Practice and Experience, 46(11), pp.1547-1569.
* Lemire D, Kaser O, Aouiche K. [Sorting improves word-aligned bitmap indexes](https://arxiv.org/abs/0901.3751). Data & Knowledge Engineering 2010; 69(1):3–28, doi:10.1016/j.datak.2009.08.006.
* Lemire D, Kaser O, Gutarra E. [Reordering rows for better compression: Beyond the lexicographical order](https://arxiv.org/abs/1207.2189). ACM Transactions on Database Systems 2012; 37(3), doi:10.1145/2338626.2338633.


## More data

If you just want short tabular datasets for machine learning purposes, there are good choices elsewhere such as [adult](https://archive.ics.uci.edu/ml/machine-learning-databases/adult/).

The [Web Table Corpora](http://webdatacommons.org/webtables/) is interesting.

See [Big Data And AI: 30 Amazing (And Free) Public Data Sources For 2018](https://www.forbes.com/sites/bernardmarr/2018/02/26/big-data-and-ai-30-amazing-and-free-public-data-sources-for-2018/#522e3e6c5f8a).

