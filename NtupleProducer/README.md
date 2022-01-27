Basic Instructions

```
cmsrel CMSSW_11_1_7
cd CMSSW_11_1_7/src
cmsenv
git cms-checkout-topic -u drankincms:btagging_CMSSW_11_1_7
git cms-addpkg  L1Trigger/TrackTrigger
git cms-addpkg SimTracker/TrackTriggerAssociation
git cms-addpkg L1Trigger/L1TMuon
git clone https://github.com/cms-l1t-offline/L1Trigger-L1TMuon.git L1Trigger/L1TMuon/data

# scripts
git clone git@github.com:drankincms/FastPUPPI.git -b 11_1_X_pfntupler

scram b -j8
```

`runL1PFNTupler_Full.py` will run directly on FEVT (or RAW)


