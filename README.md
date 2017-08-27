# Mie Theory Condensate Data

We provide tabulated data for condensates using our Mie theory code. The data include extinction cross-sections, scattering cross-sections, and asymmetry parameters. 

## Description of Condensate Data Files

We compute cross-sections and asymmetry parameters for 19 condensate species. Each condensate has its own data file labeled by *[condensate formula].data*. The structure of each data file is the same and is as follows. A data file contains the wavelengths of light in vacuum (in metres), extinction cross-sections (in square metres), scattering cross-sections (in square metres), and asymmetry parameters (dimensionless) for various modal particle sizes between 0.01 microns and 100 microns in the modified gamma distribution (see Pinhas & Madhusudhan 2017). The first column of each row contains the wavelengths. The spanned wavelength range is 0.3 to 30 microns, covering the spectral domains of the Hubble Space Telescope and the James Webb Space Telescope. The real refractive index of the ambient medium is assumed to be unity in the Mie theory calculations, such that the wavelength of light in the ambient medium surrounding the condensate particles is equal to the incident wavelength in vacuum (good approximation for an H<sub>2</sub>-dominated atmosphere). 

The subsequent columns of each row are grouped into sets corresponding to various condendate modal particle sizes, with three columns in each set. The first column of a set is the extinction cross-section, the second column is the scattering cross-section, and the third is the asymmetry parameter. The first set of three columns is for the lowest modal particle size of 0.01 microns. The next set of three columns is for the second modal particle size in {1.0 x 10<sup>-2</sup>, 1.37 x 10<sup>-2</sup>, 1.89 x 10<sup>-2</sup>, 2.59 x 10<sup>-2</sup>, 3.56 x 10<sup>-2</sup>, 4.89 x 10<sup>-2</sup>, 6.72 x 10<sup>-2</sup>, 9.24 x 10<sup>-2</sup>, 1.27 x 10<sup>-1</sup>, 1.74 x 10<sup>-1</sup> 2.40 x 10<sup>-1</sup>, 3.29 x 10<sup>-1</sup>, 4.52 x 10<sup>-1</sup>, 6.21 x 10<sup>-1</sup>, 8.53 x 10<sup>-1</sup>, 1.17 x 10<sup>0</sup>, 1.61 x 10<sup>0</sup>, 2.21 x 10<sup>0</sup>, 3.04 x 10<sup>0</sup>, 4.18 x 10<sup>0</sup>, 5.74 x 10<sup>0</sup>, 7.88 x 10<sup>0</sup>, 1.08 x 10<sup>1</sup>, 1.49 x 10<sup>1</sup>, 2.04 x 10<sup>1</sup>, 2.81 x 10<sup>1</sup>, 3.86 x 10<sup>1</sup>, 5.30 x 10<sup>1</sup>, 7.28 x 10<sup>1</sup>, 1.0 x 10<sup>2</sup>} microns. This pattern continues to the end of each row. Where experimental data of refractive indices are lacking for certain wavelengths, we set the cross-sections and asymmetry parameters to 1e-100. 

## Authors

This library of condensate data was computed using a Python Mie theory code written by Arazi Pinhas & Nikku Madhusudhan, Institute of Astronomy, Cambridge UK. 

## Citations

If this library of condensate data is useful to you, the following scientific publications should be referenced in your work:

1. Pinhas A., Madhusudhan N., On signatures of clouds in exoplanetary transit spectra, *Monthly Notices of the Royal Astronomical Society*, Volume 471, Issue 4, 11 November 2017, Pages 4355–4373, https://doi.org/10.1093/mnras/stx1849

2. Bohren C. F., Huffman D. R., 1983, Absorption and scattering of light by small particles. Wiley-VCH

3. Deirmendjian D., 1969, Electromagnetic scattering on spherical polydispersions. Elsevier
