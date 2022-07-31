![enter image description here](https://i.ibb.co/nzzs9Lb/memory-card-1.png)

# memOptix


This Jupyter notebook will assist DFIR professional in analysing the output generated from Volatility memory extraction framework in a structured manner.  Current version of the notebook is written to process Volatility output from Windows OSs. 

Please note that this notebook was created based on the output generated from CrowdStrike's Supermem python script (https://github.com/CrowdStrike/SuperMem). SuperMem triage mode 2 or 3 should be run against the memory dump prior to running this notebook.  A separate Volatility processing cell is provided as part of this notebook, if you decide to run Volatility against a memory dump interactively to generate the required output.

Following Open Source projects are used in this notebook
https://github.com/microsoft/msticpy
https://github.com/volatilityfoundation/volatility3
https://github.com/CrowdStrike/SuperMem

Author : J Marasinghe

# Pre-requisites 

 - Python 3.8 or above 
 - Volatility3  
 -  Following API keys are required to
   support MSTICPY with its enrichments. [GeoIPLite](https://dev.maxmind.com/geoip/geolite2-free-geolocation-data?lang=en), [GreyNoise](https://docs.greynoise.io/docs/getting-started) and [OTX](https://otx.alienvault.com/api)  

## Usage

1.  git clone https://github.com/blueteam0ps/memOptix.git
2. Update **msticpyconfig.yaml** and include the API keys described in the pre-requisites
3. Open the **memOptix-analyst.ipynb** within Jupyter and follow instructions within the notebook 
4. If you are not planning to run Supermem and want to generate the CSVs required for the notebook please run the following cell. If you already have the CSVs, then update the path as instructed and skip the CSV generation.

![Generate CSVs](https://github.com/blueteam0ps/memOptix/blob/main/imgs/csv-generation.jpg?raw=true)

### Screenshots 
![Network IOC enrichment](https://raw.githubusercontent.com/blueteam0ps/memOptix/main/imgs/Network%20IOC%20Enrichment.jpg?token=GHSAT0AAAAAABQPZ26W7U3SQ4VZ3GGTXJCOYXGQU4Q)

![Process Tree Visualisation](https://raw.githubusercontent.com/blueteam0ps/memOptix/main/imgs/Process%20Tree%20Visualisation%20-%20MSTICPY.jpg?token=GHSAT0AAAAAABQPZ26XX6FK4J6GH25YNDWYYXGQVWA)

![Timeseries analysis](https://raw.githubusercontent.com/blueteam0ps/memOptix/main/imgs/Timeseries%20-%20MSTICPY.jpg?token=GHSAT0AAAAAABQPZ26WI4EOPBK52S2NOYHKYXGQWLA)

Image Credit
<a href="https://www.flaticon.com/free-icons/memory" title="memory icons">Memory icons created by Darius Dan - Flaticon</a>
