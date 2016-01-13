# Approaches to automating counting wing cells on a Drosophila adult wing.

THis is currently less a protocol, and more a list of different approaches that are currently being used (along with some references)


## Manual counting

i.e. Take an image of a fixed area (10X or 20X objective) and count number of hairs. Then compute how many times this fits into a wing compartment (or other unit).  Cell size is computed by dividing cell number by compartment area.


## [FijiWings](http://www.ncbi.nlm.nih.gov/pubmed/23797110)

This is NIH IMage/Fiji set of [macros](http://sourceforge.net/projects/fijiwings/) to help capture all of the wing trichomes and estimate cell number. It is not super clear how well this works, 
it works. I have found it a bit frustrating to use. They have a [primer](https://youtu.be/kkwbRaN51ww) for Fijiwings 2.2 on youtube

## From [Torquato et al. 2014](http://link.springer.com/article/10.1007/s10709-014-9795-0/fulltext.html)
This is directly from their paper
Cell size (area) and cell number

Images of fixed-size rectangles within each intervein region (IVR) at dorsal wing surface (Fig. 1b) were captured with above mentioned digital camera (and software) on a optic microscope (Zeiss Stemi Axioskop 2) and used for trichome counting (1000× magnification; fixed rectangle area of 0.00906 mm2). Trichome counting was performed using the cell counter plugin v.2010 on ImageJ v.1.46r; all visible trichomes were counted. Given that cell density might not be homogeneous throughout the wing, we aimed at taking each rectangle image in equivalent positions for all analyzed wings. A proxy for average cell area (CA) in each IVR was estimated through the ratio between the fixed surface area of rectangle image (0.00906 mm2) and the respective number of counted trichomes (Fig. 1b). We also investigated how variation in cell area is distributed across the wing surface and whether this distribution was affected by response to artificial selection and/or temperature variation during the development (details in next section). In turn, cell number (CN) in each IVR was given by the ratio between the estimated IVR area (traced areas in Fig. 1a) and the respective CA. We note that a thorough estimation of CA and CN across the wing blade was performed by analyzing five different intervein regions, instead of using only one or two regions as commonly performed in the literature. Total cell number at dorsal wing surface (CN Total) was calculated through the ratio between the estimates of whole wing area (π × W L/2 × W W/2; a proxy to the ellipse area) and average cell area across all intervein regions (CA Average).

## Other Considerations

### Image Quality
I assume that a higher quality (and "larger") image will be best. Need to test this.

### Colour vs mono
Which is best?

### Contrast

### Depth of field

### Brightness

### Mounting media

### Objective
Assume the highest quality objective that will fit the whole wing in the field of view is best (i.e. a 4X or 5X plan apochromatic lense)

### Brightfield upright? Brightfield inverted? stereoscope (white or black background)?

