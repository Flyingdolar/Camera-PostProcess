# Image Process Pipeline Design

> Implement following Image Pipeline on CPP


## Device Calibration

> Before doing image processing, we have to adjust device so that we can do image process without side effects by devices.

1. Find the gain of Dark Current (Offset of the image)
2. Finding CCM (Color Correction Matrix)
3. Get CTC (Color Temperature Curve)

##  Image Process

> A Image Process Pipeline that render the image from raw data.

1. Remove Dark Current
2. Demosaicing
3. White balance (Remove outer light effects)
4. Apply CCM (Do color correction)
5. Tone Reproduction
   - Biateral Filter
   - Edge Extract
   - Light Adjustment
   - Align Middle Gray
   - Tone Reproduction Curve
   - Color Enhancement
6. Gamma Correction
