# OptDebug
OptDebug: Fault-Inducing Operation Isolation for Dataflow Applications (SoCC 2021)

## Summary of OptDebug
Fault-isolation is extremely challenging in large scale data processing in cloud environments. Data provenance is a dominant existing approach to isolate data records responsible for a given output. However, data provenance concerns fault isolation only in the data-space, as opposed to fault isolation in the code-space—how can we precisely localize operations or APIs responsible for a given suspicious or incorrect result?

OptDebug identifies fault-inducing operations in a dataflow application using three insights. First, debugging is easier with a small-scale input than a large-scale input. So it uses data provenance to simplify the original in- put records to a smaller set leading to test failures and test successes. Second, keeping track of operation provenance is crucial for debugging. Thus, it leverages automated taint anal- ysis to propagate the lineage of operations downstream with individual records. Lastly, each operation may contribute to test failures to a different degree. Thus OptDebug ranks each operation’s spectra—the relative participation frequency in failing vs. passing tests. In our experiments, OptDebug achieves 100% recall and 86% precision in terms of detecting faulty operations and reduces the debugging time by 17× compared to a naïve approach. Overall, OptDebug shows great promise in improving developer productivity in today’s complex data processing pipelines by obviating the need to re-execute the program repetitively with different inputs and manually examine program traces to isolate buggy code.

## Team
This project is led by Professor [Muhammad Ali Gulzar](https://people.cs.vt.edu/~gulzar/) at Virginia Tech. 

[Muhammad Ali Gulzar](https://people.cs.vt.edu/~gulzar/): Professor at Virginia Tech, gulzar@cs.vt.edu; Prof Kim's former PhD student at UCLA 

[Miryung Kim](http://web.cs.ucla.edu/~miryung/): Professor at UCLA, miryung@cs.ucla.edu;

For more information please visit this [GitHub repository](https://github.com/maligulzar/OptDebug) at Virginia Tech. 
## How to cite 
Please refer to our SoCC 2021 paper, [OptDebug: Fault-Inducing Operation Isolation for Dataflow Applications](https://people.cs.vt.edu/~gulzar/assets/pdf/optdebug_socc21.pdf) for more details. 

### Bibtex  

[DOI Link]()
