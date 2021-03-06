ImageJ Training 1 180726 by Ryosuke TAJIMA  
==============  
  
# 1. Manual measurement  
## 1-1. Line measurement  
1. Open image  
1. Use zoom in / out: Image > Zoom  
    Shortcut keys are usuful. (higly recomendation)
1. Select "line tool"  
1. Trace with straight line  
1. Measure: Analyse > Measure  
    The values were expressed as pixels.  
1. Estimation:  
    Using dpi of image at the time of taking image  
    Or compare with the scale in same or different photo  
  
## 1-2. Segmented line measurement  
1. Select segmented: right-click "line tool"  
1. Trace with segmented line  
1. Measure: Analyse > Measure  
Length value is adjusted how pixels connect  
  
## 1-3. Area measurement  
1. Select "Polygon tool"  
1. Trace with segmented line  
1. Measure: Analyse > Measure  
    It can measure not only area but perimeter, major and minor (in ellipse approximation)  
  
## 1-4. Ohter usuful measurement
1. Select "Angle tool"  
1. Select "Multi-point tool"  
  
# 2. Using analyse particle  
## 2-1. Basic
1. Change color image to grayscale: Image > Type > 8bit 
1. Thresholding: Image > Adjust > Threshold  
The threshold value are manually or autmatically selected.  
1. Apply: Click "Apply"  
1. Analyze Particle: Analyze > Analyze Particle  
1. Check the left side boxes and Uncheck the rightside boxes (my recommendation)  
1. Set size and circularity  
    Size: the range of wanted size  
    Circularity: the range of near-circular particle  
1. Click "OK"  
  
## 2-2. Mind the color (analyse using RGB)
1. Split RGB: Image > Color > Split channels  
1. Select good image  
1. Thresholding: Image > Adjust > Threshold
1. Sometimes use invert: Edit > Invert  
1. Analyze Particle: Analyze > Analyze Particle  
    For coverage, use summarize and image size  
1. Use image calculator: Process > Image calculator  
    e.g.leaf senescence  

## 2-3. Measure root length  
1. Thresholding:  Image > Adjust > Threshold  
1. Remove pixels from the edges: Process > Binary > Erode  
1. Add pixels to the edges: Process > Binary > Dilate  
1. Remove pixels from the edges until single-pixel wide: Process > Binary > Skeletonize  
1. Analyze Particle: Analyze > Analyze Particle (more than 2pixels)  
1. Estimation root length: values x 1.1 / 400 x 2.54  
    400 dpi, 2.54 cm / inch  
    1.1 as the factor for rough calculation  
  
# 3. Get Histogram  
1. Split RGB: Image > Color > Split channels  
1. Select good image  
1. Get histgram: Analyze > histgram  
1. Get and use the list of histgram: Click "List"  
    The datasets of hitgram is often big. it' analysed using R.

