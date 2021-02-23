# k-means


Implement the k-means clustering algorithm and apply it to color a given image (paris.png). 

1) Use the following code to load the image. 
It will return a (244, 198, 3) numpy.ndarray. 
The first two dimensions represent the height and width of the image. The last dimension represents the 3 color channels (RGB) for each pixel of the image. 

  import skimage.io
  import matplotlib.pyplot as plt
  img = skimage.io.imread(’image.png’)
  skimage.io.imshow(img)
  plt.show()
  
2) Implement the k-means algorithm to partition the 244×198 pixels into k clusters based on their RGB values and the Euclidean distance measure. Run your experiment with k = 2, 3, 6, 10 with the following given starting centroids: 
k = 2: (0, 0, 0), (0.1, 0.1, 0.1)
k = 3: (0, 0, 0), (0.1, 0.1, 0.1), (0.2, 0.2, 0.2)
k = 6: (0, 0, 0), (0.1, 0.1, 0.1), (0.2, 0.2, 0.2), (0.3, 0.3, 0.3), (0.4, 0.4, 0.4), (0.5, 0.5, 0.5)
k = 10: (0, 0, 0), (0.1, 0.1, 0.1), (0.2, 0.2, 0.2), (0.3, 0.3, 0.3), (0.4, 0.4, 0.4), (0.5, 0.5, 0.5), (0.6, 0.6, 0.6), (0.7, 0.7, 0.7), (0.8, 0.8, 0.8), (0.9, 0.9, 0.9) 

For each value of k, you will run k-means until either convergence or your program has conducted 50 iterations over the data, whichever comes first. 

Deliverables: 
For each k = 2,3,6,10, report the final SSE and re-color the pixels in each cluster using the following color scheme: 
  Cluster 1. SpringGreen: (60, 179, 113)
  Cluster 2. DeepSkyBlue: (0, 191, 255)
  Cluster 3. Yellow: (255, 255, 0)
  Cluster 4. Red: (255, 0, 0)
  Cluster 5. Black: (0, 0, 0)
  Cluster 6. DarkGray: (169, 169, 169)
  Cluster 7. DarkOrange: (255, 140, 0)
  Cluster 8. Purple: (128, 0, 128)
  Cluster 9. Pink: (255, 192, 203)
  Cluster 10. White: (255, 255, 255)
