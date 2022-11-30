# This repo serves as the report and codebase for Lab 1/3 for the Advanced Computer Architecture course, on the Electrical and Computer Engineering school of Aristotle University of Thessaloniki

Ανδρονίκου Δημήτρης, 9836

Αλεξανδρίδης Φώτιος, 9953

---
## Advaced Computer Architecture, Lab 02

### Question 1

#### Subquestion a

L1 instruction   *=> size=32768 ~> 32KB*

associativity *assoc=2*

L1 Data caches  *=> size=65536 ~> 65 KB*

associativity *assoc=2*

L2 cache *size=2097152  ~>  2MB*

associativity *assoc=8*

cache line	cache\_line\_size=64

#### Subquestion b

##### Specbzip
1) χρόνο εκτέλεσης			*sim\_seconds  =  0.083982*
1) CPI 					*system.cpu.cpi  =  1.679650*

1) συνολικά miss rates για την L1 Instruction cache *system.cpu.icache.overall\_miss\_rate::total     0.000077*

1) συνολικά miss rates για την L1 Data cache *system.cpu.dcache.overall\_miss\_rate::total     0.014798*

1) συνολικά miss rates για την L2 cache 

*system.l2.overall\_miss\_rate::total           0.282163*

##### Specmcf
1) χρόνο εκτέλεσης			*sim\_seconds  =  0.064955*
1) CPI 					*system.cpu.cpi  =  1.299095*

1) συνολικά miss rates για την L1 Instruction cache *system.cpu.icache.overall\_miss\_rate::total     0.023612*

1) συνολικά miss rates για την L1 Data cache *system.cpu.dcache.overall\_miss\_rate::total     0.002108*

1) συνολικά miss rates για την L2 cache 

*system.l2.overall\_miss\_rate::total           0.055046*

##### Spechmmer
1) χρόνο εκτέλεσης			*sim\_seconds  =  0.059396*
1) CPI 					*system.cpu.cpi  =  1.187917*

1) συνολικά miss rates για την L1 Instruction cache *system.cpu.icache.overall\_miss\_rate::total     0.000221*

1) συνολικά miss rates για την L1 Data cache *system.cpu.dcache.overall\_miss\_rate::total     0.001637*

1) συνολικά miss rates για την L2 cache 

*system.l2.overall\_miss\_rate::total           0.077760*

##### Specsjeng
1) χρόνο εκτέλεσης:			*sim\_seconds  =  0.513528*
1) CPI: 					*system.cpu.cpi  =  10.270554*

1) συνολικά miss rates για την L1 Instruction cache: *system.cpu.icache.overall\_miss\_rate::total     0.000020*

1) συνολικά miss rates για την L1 Data cache: *system.cpu.dcache.overall\_miss\_rate::total     0.121831*

1) συνολικά miss rates για την L2 cache: 

*system.l2.overall\_miss\_rate::total           0.999972*

##### Speclibm
1) χρόνο εκτέλεσης:			*sim\_seconds  =  0.174671*
1) CPI: 					*system.cpu.cpi  =* *3.493415*

1) συνολικά miss rates για την L1 Instruction cache: *system.cpu.icache.overall\_miss\_rate::total     0.000094*

1) συνολικά miss rates για την L1 Data cache: *system.cpu.dcache.overall\_miss\_rate::total     0.060972*

1) συνολικά miss rates για την L2 cache: 

*system.l2.overall\_miss\_rate::total           0.999944*


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specmcf</h2>|<h2>Spechmmer</h2>|<h2>Specsjeng</h2>|<h2>Speclibm</h2>|
| :- | :- | :- | :- | :- | :- |
|χρόνος εκτέλεσης|0.083982|0.064955|0.059396|0.513528|0.174671|


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specmcf</h2>|<h2>Spechmmer</h2>|<h2>Specsjeng</h2>|<h2>Speclibm</h2>|
| :- | :- | :- | :- | :- | :- |
|CPI|1.679650|1.299095|1.187917|10.270554|3.493415|


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specmcf</h2>|<h2>Spechmmer</h2>|<h2>Specsjeng</h2>|<h2>Speclibm</h2>|
| :- | :- | :- | :- | :- | :- |
|*Icache\_miss\_rate::total*|0.000077|0.023612|0.000221|0.000020|0.000094|


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specmcf</h2>|<h2>Spechmmer</h2>|<h2>Specsjeng</h2>|<h2>Speclibm</h2>|
| :- | :- | :- | :- | :- | :- |
|*dcache\_miss\_rate::total*|0.014798|0.002108|0.001637|0.121831|0.060972|


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specmcf</h2>|<h2>Spechmmer</h2>|<h2>Specsjeng</h2>|<h2>Speclibm</h2>|
| :- | :- | :- | :- | :- | :- |
|*l2\_miss\_rate::total*|0.282163|0.055046|0.077760|0.999972|0.999944|

![](Aspose.Words.f3488851-f0ed-4cf6-b351-049795c663bc.001.png)

1.	Ο χρόνος εκτέλεσης του specsjeng είναι πολύ μεγαλύτερος από των άλλων

![](Aspose.Words.f3488851-f0ed-4cf6-b351-049795c663bc.002.png)

2.	Το CPI του specsjeng είναι πολύ μεγαλύτερο από των άλλων


![](Aspose.Words.f3488851-f0ed-4cf6-b351-049795c663bc.003.png)

3.	Όμως το miss rate των instructions του specmcf είναι πολύ μεγαλύτερο από των άλλων

![](Aspose.Words.f3488851-f0ed-4cf6-b351-049795c663bc.004.png)

4.	Το miss rate των data του specsjeng είναι πολύ μεγαλύτερο από των άλλων


![](Aspose.Words.f3488851-f0ed-4cf6-b351-049795c663bc.005.png)

5.	Το miss rate στην L2 του specsjeng και του speclibm είναι πολύ μεγαλύτερα από των άλλων

Λόγω του 5 και του 4 είναι λογικό να προκύψει μεγάλο CPI για το specsjeng, άρα και μεγάλος χρόνος εκτέλεσης.

#### Subquestion c

`system.clk_domain.clock` entry
| | 401.bzip2 | 429.mcf | 456.hmmer | 458.sjeng | 470.lbm | 
| --- | --- | --- | --- | -- | --- |
| default | 1000 | 1000 | 1000 | 1000 | 1000 |
| 1GHz | 1000 | 1000 | 1000 | 1000 | 1000 |
| 3GHz | 1000 | 1000 | 1000 | 1000 | 1000 |

`cpu_cluster.clk_domain.clock` entry
| | 401.bzip2 | 429.mcf | 456.hmmer | 458.sjeng | 470.lbm | 
| --- | --- | --- | --- | -- | --- |
| default | 500 | 500 | 500 | 500 | 500 |
| 1GHz | 1000 | 1000 | 1000 | 1000 | 1000 |
| 3GHz | 333 | 333 | 333 | 333 | 333 |

To answer the theretical questions, we will focus on the first benchmark, but the same information is appliccable for all benchmarks.
We observe that the system clock entry defines the clock rate for the total system, the components of the motherboard. The CPU clock is responsible for defining the clock rate for the different CPU components. Because a CPU usually has to perform more operations per unit of time compared to the other components, the CPU clock is usually defined to be at least as fast as the system clock, but usually faster. For performance and syncronization reasons, we actually want the system clock rate in
ticks to be an integral product of the CPU clock rate in ticks. By inspecting the `config.json` file for a 1GHz benchmark, we can observe that the different CPU components are clocked according to the CPU clock rate. For a MinorCPU model (defined in the commands we use to run the benchmarks), these components are:

1. L1 data cache (dcache)
2. L1 instruction cache (icache)
3. L2 cache
4. Instruction walker cache
5. Data walker cache
6. Data busses that connect the components mentioned above

If we add another CPU, meaning we add another core to the CPU cluster, its clock rate will be the defined CPU clock rate, always according to its architecture.

For the scaling we have the following execution times for the 1GHz and 3GHz simulations:

Simulation time (in seconds)
| | 401.bzip2 | 429.mcf | 456.hmmer | 458.sjeng | 470.lbm | 
| --- | --- | --- | --- | -- | --- |
| 1GHz | 0.165228 | 0.124137 | 0.118530 | 0.329087 | 0.246976 |
| 3GHz | 0.061589 | 0.043909 | 0.039646 | 0.138401 | 0.135953 |

As we can observe from the table, in some cases the scaling is better than the others (specifically, in benchmark 456.hmmer we can see that the rate is closer to 3 than in 470.lbm). Achieving perfect scaling is close to impossible, because the system performance depends on a lot of parameters other than CPU clock (for example: cache line size).

#### Subquestion d

##### Specbzip
1) χρόνο εκτέλεσης:			*sim\_seconds  =  0.083609*
1) CPI: 					*system.cpu.cpi  =  1.672175*

1) συνολικά miss rates για την L1 Instruction cache: *system.cpu.icache.overall\_miss\_rate::total     0.000077*

1) συνολικά miss rates για την L1 Data cache: *system.cpu.dcache.overall\_miss\_rate::total     0.014795*

1) συνολικά miss rates για την L2 cache: 

*system.l2.overall\_miss\_rate::total           0.282159*


|<h2></h2>|<h2>Specbzip</h2>|<h2>Specbzip(fast DDR)</h2>|<h2>%</h2>|
| :- | :- | :- | :- |
|χρόνος εκτέλεσης|0.083982|0.083609|-0.4441|
|` `CPI|1.679650|1.672175|-0.4465|
|*Icache\_miss\_rate::total*|0.000077|0.000077|0|
|*dcache\_miss\_rate::total*|0.014798|0.014795|-0.02|
|*l2\_miss\_rate::total*|0.282163|0.282159|-0.0014|



Παρατηρούμε ότι με την αύξηση της συχνότητας της μνήμη μειώνεται το miss rate για την L2 και την L1 data cache. Αυτό είναι λογικό διότι αυτές οι caches θα λαμβάνουν δεδομένα πιο γρήγορα, άρα θα έχουμε λιγότερα misses στον ίδιο χρόνο. Αυτό έχει επίδραση στο CPI, που είναι λογικό, και φυσικά το CPI όπως φάνηκε και προηγουμένως επηρεάζει σχεδόν ανάλογα τον χρόνο εκτέλεσης.


### Question 2

### Bibliography

1. [http://pages.cs.wisc.edu/~david/courses/cs752/Fall2015/gem5-tutorial/index.html](http://pages.cs.wisc.edu/~david/courses/cs752/Fall2015/gem5-tutorial/index.html)
2. [https://www.gem5.org/documentation/](https://www.gem5.org/documentation/)
