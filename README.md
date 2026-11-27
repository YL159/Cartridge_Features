## Cartridge Case Masking Methods

This project is intended to showcase bullet cartridge case image processing methods and results.

#### Dataset information
Open source dataset:<br>
[NIST Ballistics Toolmark Research Database (NBTRD)](https://tsapps.nist.gov/NRBTD/)

Search: https://tsapps.nist.gov/NRBTD/Studies/Search<br>
Nominal Caliber: 9mm<br>
Measurand: Photo Image

Study Name: Hamby Hi-Point C9 Slides<br>
Study Description: 30 Cartridge cases fired from ten consecutively manufactured Hi-Point C9 pistol slides.<br>
Link: https://tsapps.nist.gov/NRBTD/Studies/Studies/Details/4908a64a-702c-4203-a945-6279df3acf3f?nm=True&mt=7&m=1&sp=1<br>
Caliber: 9mm Luger

Image file name abbr:<br>
BF R: Breech Face, Ring light. This provides uniformed image feature brightness.

#### Methods
1. Breech face & firing pin impression: Hough Circle Transform with tuned parameters.
2. Aperture shear: Hough Line Transform with tuned parameters, line histogram categorization and heatmap threshold contour presentation.
3. Firing pin shear & drag: Reuse firing pin Hough Circle, polar warp transform the circle band, detect the largest weak gradient zone as pin shear area. Not implemented because lack of meaningful dataset.

#### Usage
1. Install required modules & libs using "requirements.txt" or "pyproject.toml"
2. In "Cartridge_features.ipynb", select target python kernel and run


#### AI assistance declaration
1. Library documentation explanation & function usage templates
2. Helped with algorithm detail & refinement
3. Numpy code style optimization