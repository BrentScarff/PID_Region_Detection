# PID_Region_Detection
Uses OpenCV's MSER (Maximally Stable Extremal Regions) alogrithm to detect blobs in flow diagrams.  Bounding boxes are filtered based on size
and merged to eliminate overlap.  By detecting blobs it was attempted to identify instrument blocks. This does not work well for flow sheets 
due to the overlap of text, lines and shape pixels resulting in blobs that combine multiple objects and not individual components as desired.  
Due to the uniformity of lines within flow sheets erosion, dilation image preprocessing does not work to disconnect regions and contour and connected
components results in the same short comings again due to connected pixels between objects.
