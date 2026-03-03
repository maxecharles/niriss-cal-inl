# NIRISS-cal-INL
### Calibrating the JWST NIRISS analog-to-digital converter (ADC) periodic integral nonlinearity (INL)

In this repository, you will find a script to correct the raw, uncalibrated (Stage 0) data from the JWST's NIRISS instrument from a systematic which was originally found by [Desdoigts et al. 2025](https://arxiv.org/abs/2510.09806) and described in detail in Dholakia et al. 2026 (submitted). This issue imprints a periodic residual of 1024 in raw analog-to-digital units (ADU) onto every observation taken by NIRISS. 



How to install and run this script:

### Install:

### Running the script:

Let's say I have uncalibrated NIRISS data in the directory /Users/shashank/Downloads/MAST_2025-04-04T06_30_06.094Z, under which exist subdirectories containing only the raw data as fits files. I want to save the output data to the folder /Users/shashank/Downloads/calibrated-output/ In a terminal under the niriss-cal-inl directory, run the calibrate_inl.py file as follows:
```
python calibrate_inl.py /Users/shashank/Downloads/MAST_2025-04-04T06_30_06.094Z/ /Users/shashank/Downloads/calibrated-output/
```

That's it! The data will be saved with the same file names in the output directory. 