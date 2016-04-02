# Approaches to optimizing counting wing cells (trichomes) on adult Drosophila wings.

THis is currently less a protocol, and more a list of different approaches that are currently being used (along with some references)

## Trichomes are on both the dorsal and ventral surface
Keep in mind that the adult Drosophila wing has both a dorsal and ventral surface. Each surface has trichomes. In our lab our protocol is to mount the wings ventral side down (ventral side facing the slide, dorsal side facing cover slip). This means that when we are imaging it on an upright microscope, the dorsal side of the wing will have the highest image quality. However, if *depth of field* is too high you may take an image with trichomes from both the dorsal and ventral surface.

![Dorsal and Ventral surfaces of the Drosophila wing. From Marcus 2001. J. Anat. 199, pg 211-216](https://github.com/DworkinLab/Protocols/blob/master/Marcus2001_Wing.png =100x "Dorsal and Ventral surfaces of the Drosophila wing. From Marcus 2001. J. Anat. 199, pg 211-216")

The figure above (Marcus 2001, J. Anatomy 199:211-216), shows an adult Drosophila wing. The filled (darkened) lines are veins on the dorsal side of the wings, with the unfilled lines being on the ventral side of the wing.

## Manual counting

i.e. Take an image of a fixed area (10X or 20X objective) and count number of hairs. Then compute how many times this fits into a wing compartment (or other unit).  Cell size is computed by dividing cell number by compartment area. There are many papers that do this (including contemporary ones). Apparently this goes back to Dobzhansky 1929!

## [FijiWings](http://www.ncbi.nlm.nih.gov/pubmed/23797110)

This is NIH IMage/Fiji set of [macros](http://sourceforge.net/projects/fijiwings/) to help capture all of the wing trichomes and estimate cell number. It is not super clear how well this works, 
it works. I have found it a bit frustrating to use. They have a [primer](https://youtu.be/kkwbRaN51ww) for Fijiwings 2.2 on youtube

## From [Torquato et al. 2014](http://link.springer.com/article/10.1007/s10709-014-9795-0/fulltext.html)
This is directly from their paper
Cell size (area) and cell number

Images of fixed-size rectangles within each intervein region (IVR) at dorsal wing surface (Fig. 1b) were captured with above mentioned digital camera (and software) on a optic microscope (Zeiss Stemi Axioskop 2) and used for trichome counting (1000× magnification; fixed rectangle area of 0.00906 mm2). Trichome counting was performed using the cell counter plugin v.2010 on ImageJ v.1.46r; all visible trichomes were counted. Given that cell density might not be homogeneous throughout the wing, we aimed at taking each rectangle image in equivalent positions for all analyzed wings. A proxy for average cell area (CA) in each IVR was estimated through the ratio between the fixed surface area of rectangle image (0.00906 mm2) and the respective number of counted trichomes (Fig. 1b). We also investigated how variation in cell area is distributed across the wing surface and whether this distribution was affected by response to artificial selection and/or temperature variation during the development (details in next section). In turn, cell number (CN) in each IVR was given by the ratio between the estimated IVR area (traced areas in Fig. 1a) and the respective CA. We note that a thorough estimation of CA and CN across the wing blade was performed by analyzing five different intervein regions, instead of using only one or two regions as commonly performed in the literature. Total cell number at dorsal wing surface (CN Total) was calculated through the ratio between the estimates of whole wing area (π × W L/2 × W W/2; a proxy to the ellipse area) and average cell area across all intervein regions (CA Average).

## Other Considerations

### Image Quality
Our tests demonstrate (to no surprise) that using digital images with maximum resolution is best.

### Colour vs mono
Which is best? Still figuring this out (ID  - April 2016).

### Bit Depth on images
(8 vs 16) - Still testing.

### Contrast
- Our tests suggest that setting up Kohler Illumination (i.e. proper set up of the field diaphragm at the light source) is very helpful. Keep in mind that the maximum field of view (when opening up the field diaphragm) is for the camera, not the ocular (eye piece).
- 
### Depth of field
- We have done some tests on our LeicaM125 Stereoscope (25X and 50X total magnification in colour and monochrome). We noticed that when the iris diaphram is 100% open (so more light, but less depth of field) we seem to get much sharper deliniation of the trichomes. At first this seemed odd to me, but likely the increase in depth of field means that the image is averaging across across a greater depth. If the trichomes are really lying in a single plane, then it would be best to have low depth of field (but fine focusing). It is also worth noting that even at the highest magnification (100X total in the ocular, 50X in the camera), it is probably not close enough for a very small (within compartment image). Probably worth trying a brightfield with 20X objective (200X total).


### Brightness
TBD
### Mounting media
- So far we have only tested our standard mounting media (70% glycerol in water with a drop of phenol to prevent micro-organism growth). 
- 
### Objective
Assume the highest quality objective that will fit the whole wing in the field of view is best (i.e. a 4X  apochromatic lense). We are testing whether a 10X objective may be better (although depth of field, and seperating dorsal from ventral views of the wing is less clear).

### Brightfield upright? Brightfield inverted? stereoscope (white or black background)?
- In terms of white vs black background (at least using the standard backgrounds), the black background for the M125 stereoscope (reflected light) was **useless** for counting trichomes.
- Our Brightfield upright (Olympus BX43) seems to produce clear images with high resolution.

## Not all regions of the adult wing have the same cell density
If you are doing small regions of images (i.e. 75px^2) then keep in mind different regions of the adult wing vary in cell density (add ref).
