# This repo serves as the report and codebase for Lab 2/3 for the Advanced Computer Architecture course, on the Electrical and Computer Engineering school of Aristotle University of Thessaloniki

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


# Questions 2
- In set associative cache, block size does not affect cache tag anyhow.
- A smaller cache tag ensures a lower cache hit time.
- A smaller cache block incurs a lower cache miss penalty.

Also

- **Increase cache line size**
  - Reduces compulsory misses
  - Reduces the miss rate
  - Increases capacity and conflict misses
- **Increase size of the cache**
  - Increases hit time, increases power consumption
  - Reduces the miss rate (it can load more Bytes on caches)
- **Higher associativity**
  - Reduces conflict misses
  - Reduces the miss rate
  - Increases hit time, increases power consumption
- **Higher number of cache levels**
  - Reduces overall memory access time
  - Reduces the miss penalty

So our run tests are these:

|Run #|L1 dcache size|L1 icache size|L2 cache size|L1 icache associat.|L1 dcache associat.|L2 cache associat.|Cache line size|
| :- | :- | :- | :- | :- | :- | :- | :- |
|1|64|64|1|1|1|2|128|
|2|64|128|2|1|1|2|32|
|3|128|64|2|1|1|2|32|
|4|128|128|4|1|1|2|128|
|5|128|128|4|2|1|2|128|
|6|128|128|4|4|1|2|128|
|7|128|128|4|4|2|2|128|
|8|128|128|4|4|4|2|64|
|9|128|128|4|4|4|4|64|
|10|128|128|4|4|4|8|128|






The results:
# Specbzip

|<h2></h2>|<h2>cpi</h2>|<h2>dcache\_miss\_rate</h2>|<h2>icache \_miss\_rate</h2>|<h2>L2 \_miss\_rate</h2>|
| :- | :- | :- | :- | :- |
|run1|1.551542|0.009703|0.000046|0.204023|
|run2|1.790627|0.018864|0.000069|0.384215|
|run3|1.756071|0.015868|0.000070|0.465377|
|run4|1.574223|0.011891|0.000047|0.166513|
|run5|1.574144|0.011891|0.000046|0.166506|
|run6|1.574144|0.011891|0.000046|0.166510|
|run7|1.556731|0.010273|0.000046|0.192764|
|run8|1.597712|0.010896|0.000057|0.312559|
|run9|1.597876|0.010896|0.000057|0.312993|
|run10|1.551542|0.009703|0.000046|0.204023|

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.006.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.007.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.008.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.009.png)
# Specmcf

|<h2></h2>|<h2>cpi</h2>|<h2>dcache\_miss\_rate</h2>|<h2>icache \_miss\_rate</h2>|<h2>L2 \_miss\_rate</h2>|
| :- | :- | :- | :- | :- |
|run1|1.181221|0.001966|0.000016|0.758297|
|run2|1.335364|0.018105|0.000055|0.316779|
|run3|2.143559|0.005244|0.103163|0.042156|
|run4|1.184956|0.002541|0.000036|0.578237|
|run5|1.184904|0.002541|0.000023|0.581209|
|run6|1.184816|0.002541|0.000016|0.583029|
|run7|1.182096|0.002097|0.000016|0.705200|
|run8|1.203137|0.003132|0.000022|0.863710|
|run9|1.203047|0.003132|0.000022|0.863262|
|run10|1.181221|0.001966|0.000016|0.758297|
#
![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.010.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.011.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.012.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.013.png)
# Spechmmer


|<h2></h2>|<h2>cpi</h2>|<h2>dcache\_miss\_rate</h2>|<h2>icache \_miss\_rate</h2>|<h2>L2 \_miss\_rate</h2>|
| :- | :- | :- | :- | :- |
|run1|1,178110|0,000367|0,000056|0,200911|
|run2|1,210302|0,004346|0,000401|0.054981|
|run3|1,194226|0,002259|0,000420|0,102704|
|run4|1,186298|0,001133|0,000334|0,056418|
|run5|1,185588|0,001133|0,000057|0,061388|
|run6|1,185588|0,001133|0,000056|0,061400|
|run7|1,178295|0,000387|0,000056|0,187128|
|run8|1,182888|0,000662|0,000078|0,208062|
|run9|1,182888|0,000662|0,000078|0,208062|
|run10|1,178110|0,000367|0,000056|0,200911|

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.014.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.015.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.016.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.017.png)
# Specsjeng

|<h2></h2>|<h2>cpi</h2>|<h2>dcache\_miss\_rate</h2>|<h2>icache \_miss\_rate</h2>|<h2>L2 \_miss\_rate</h2>|
| :- | :- | :- | :- | :- |
|run1|3.348858|0.248364|0.011330|0.044292|
|run2|5.605595|0.393710|0.003321|0.290642|
|run3|5.684481|0.392898|0.012986|0.123246|
|run4|3.261793|0.243757|0.002443|0.166720|
|run5|3.251312|0.243745|0.000578|0.288207|
|run6|3.247843|0.243744|0.000115|0.352064|
|run7|3.240343|0.242518|0.000114|0.702941|
|run8|3.173673|0.243469|0.000108|0.894077|
|run9|3.173692|0.243468|0.000108|0.894172|
|run10|3.239587|0.242393|0.000114|0.780786|

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.018.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.019.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.020.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.021.png)
# Speclibm

|<h2></h2>|<h2>cpi</h2>|<h2>dcache\_miss\_rate</h2>|<h2>icache \_miss\_rate</h2>|<h2>L2 \_miss\_rate</h2>|
| :- | :- | :- | :- | :- |
|run1|1.883187|0.032168|0.000102|0.944590|
|run2|3.648170|0.123694|0.000071|0.997075|
|run3|3.648098|0.123577|0.000075|0.998511|
|run4|1.874379|0.031517|0.000089|0.971545|
|run5|1.874379|0.031517|0.000087|0.971559|
|run6|1.874379|0.031517|0.000086|0.971562|
|run7|1.865695|0.030867|0.000086|0.999997|
|run8|2.467162|0.061731|0.000085|0.999999|
|run9|2.467162|0.061731|0.000085|0.999999|
|run10|1.865695|0.030867|0.000086|0.999997|

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.022.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.023.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.024.png)

![](Aspose.Words.fe4960a9-4620-4b93-b72f-0a01780ebd0e.025.png)

Overall, we can see that we achieve the lowest CPI consistently across all benchmarks on runs 1, 7 and 10. We can definitely conclude that a higher cache line size is vital to lowering CPI, since for the runs with the smaller sizes (32) we can consistently see the highest CPI there along every benchmark. Apart from that we can see that increasing associativity has a minimal effect on CPI, by checking the differences between the three runs. Cache size doesn’t impact the CPI much.

As such, we can conclude that the CPI is largely impacted by cache line size (higher -> better CPI), impacted somewhat by associativity (higher -> better CPI) and is marginally impacted by cache sizes (higher -> better CPI in some cases).
# Question 3

Θέλουμε μια συνάρτηση Απόδοση/Κόστος, όπου Απόδοση = 1/CPI και Κόστος = Cost

Άρα η F = 1CPICost=1CPI\*Cost

Θέλουμε να την μεγιστοποιήσουμε, άρα να ελαχιστοποιήσουμε το CPI\*Cost

To Cost ορίζεται ως εξής:

Cost = 10\*cost\_L1\_data + 10\*cost\_L1\_instr + cost\_L2 + 10\*cost\_L1\_data\_asso + 10\*cost\_L1\_inst\_asso + cost\_L2\_asso + cost\_line\_s
όπου cost\_L1\_data = μέγεθος της L1 data 
όπου cost\_L1\_instr = μέγεθος της L1 instruction
όπου cost\_L2 = μέγεθος της L2
όπου cost\_L1\_data\_asso = μέγεθος του L1 data associativity 
όπου cost\_L1\_inst\_asso = μέγεθος του L1 instruction associativity 
όπου cost\_L2\_asso = μέγεθος του L2 associativity 
όπου cost\_line\_s = μέγεθος του cache line 

το x10 το χρησιμοποιήσαμε διότι το κόστος της L1 είναι πολύ μεγαλύτερο από της L2

## Cost(run-i)

|run1|2430|
| :- | :- |
|run2|3974|
|run3|3974|
|run4|6710|
|run5|6720|
|run6|6740|
|run7|6750|
|run8|6706|
|run9|6708|
|run10|6776|

Και το Cost = Cost /1000 (ώστε να είναι ίδια τάξη μεγέθους με το cpi) 
# Specbzip

|<h2></h2>|<h2>F</h2>|
| :- | :- |
|run1|0.265234|
|run2|0.140529|
|run3|0.143295|
|run4|0.09467|
|run5|0.094534|
|run6|0.094253|
|run7|0.095166|
|run8|0.093333|
|run9|0.093296|
|run10|0.095119|




# Specmcf

|<h2></h2>|<h2>F</h2>|
| :- | :- |
|run1|0.34839|
|run2|0.18844|
|run3|0.11739|
|run4|0.12577|
|run5|0.12559|
|run6|0.12522|
|run7|0.12533|
|run8|0.12394|
|run9|0.12392|
|run10|0.12494|

# Spechmmer

|<h2></h2>|<h2>F</h2>|
| :- | :- |
|run1|0.34931|
|run2|0.20791|
|run3|0.21071|
|run4|0.12563|
|run5|0.12552|
|run6|0.12514|
|run7|0.12573|
|run8|0.12606|
|run9|0.12603|
|run10|0.12527|

# Specsjeng

|<h2></h2>|<h2>F</h2>|
| :- | :- |
|run1|0.12288|
|run2|0.04489|
|run3|0.04427|
|run4|0.04569|
|run5|0.04577|
|run6|0.04568|
|run7|0.04572|
|run8|0.04699|
|run9|0.04697|
|run10|0.04556|





# Speclibm

|<h2></h2>|<h2>F</h2>|
| :- | :- |
|run1|0.21852|
|run2|0.06898|
|run3|0.06898|
|run4|0.07951|
|run5|0.07939|
|run6|0.07916|
|run7|0.07941|
|run8|0.06044|
|run9|0.06042|
|run10|0.0791|

Άρα καλύτερη επιλογή για όλα run 1 κυρίως λόγω πολύ χαμηλού κόστους και καλού cpi, παρόλο που οι άλλες δοκιμές έχουν περισσότερη cache memory δεν έχουν καλύτερο cpi.
# Bibliography
<https://www.gatevidyalay.com/cache-line-cache-line-size-cache-memory/>

<http://ece-research.unm.edu/jimp/611/slides/chap5_4.html>

Computer Architecture John L. Hennesy and A. Patterson, 4th edition

