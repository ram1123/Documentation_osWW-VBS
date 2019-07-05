**Table of content**

# Official Recommendation

1. For 2016: [https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2016Analysis](https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2016Analysis)
2. For 2017: [https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2017Analysis](https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2017Analysis)
3. For 2018: [https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2018Analysis](https://twiki.cern.ch/twiki/bin/viewauth/CMS/PdmV2018Analysis)

# How to calulate luminosity

1. Load cms enviornment using `cmsenv`.
2. Set the brilcal environment:
   ```bash
   export PATH=$HOME/.local/bin:/cvmfs/cms-bril.cern.ch/brilconda/bin:$PATH
   ```
3. Get the luminosity:
   ```bash
   brilcalc lumi --normtag /cvmfs/cms-bril.cern.ch/cms-lumi-pog/Normtags/normtag_PHYSICS.json -u /fb  -i /afs/cern.ch/user/r/rasharma/public/temp/processedLumis.json
   ```

**NOTE**: *For some reason this brilcalc command is not working on lpc. But it works fine on lxplus.*

# Reference

1. [https://twiki.cern.ch/twiki/bin/view/CMS/BrilcalcQuickStart](https://twiki.cern.ch/twiki/bin/view/CMS/BrilcalcQuickStart)
2. [Luminosity physics group](https://twiki.cern.ch/twiki/bin/view/CMS/TWikiLUM)
3. [CMS Luminosity public plots](https://twiki.cern.ch/twiki/bin/view/CMSPublic/LumiPublicResults)
2. [https://hypernews.cern.ch/HyperNews/CMS/get/physics-validation/3358.html](https://hypernews.cern.ch/HyperNews/CMS/get/physics-validation/3358.html)

