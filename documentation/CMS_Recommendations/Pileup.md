#### Table of Content

- [Pile-up](#pile-up)
    - [POG Recipes for Moriond 2017](#pog-recipes-for-moriond-2017)
    - [How To Make PU Distribution for data](#how-to-make-pu-distribution-for data)

---

# Pile-up

https://twiki.cern.ch/twiki/bin/view/CMS/PileupJSONFileforData

## POG Recipes for Moriond 2017

* Pile-up reweighting xsec = 69.2mb

Ref: https://twiki.cern.ch/twiki/bin/viewauth/CMS/POGRecipesICHEP2016

## How To Make PU Distribution for data

Command to run:
```bash
pileupCalc.py -i MyAnalysisJSON.txt --inputLumiJSON pileup_latest.txt  --calcMode true --minBiasXsec 69200 --maxPileupBin 50 --numPileupBins 50  MyDataPileupHistogram.root
```
where,
* MyAnalysisJSON.txt is the JSON file we are using. Generally it should be the golden JSON.
* pileup_latest.txt : this is input json file. It can be found at link: /afs/cern.ch/cms/CAF/CMSCOMM/COMM_DQM/certification/Collisions15/13TeV/PileUp/pileup_latest.txt

Reference: https://twiki.cern.ch/twiki/bin/viewauth/CMS/PileupJSONFileforData#Pileup_JSON_Files_For_Run_II
