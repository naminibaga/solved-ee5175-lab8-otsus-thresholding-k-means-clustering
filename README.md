Download Link: https://assignmentchef.com/product/solved-ee5175-lab8-otsus-thresholding-k-means-clustering
<br>
Otsu’s thresholding &amp; K-Means Clustering

<ol>

 <li>Calculate the global threshold value of the given images pgm and palmleaf2.pgm using Otsu’s thresholding algorithm, and display the thresholded binary images. Comment on your observations.</li>

 <li>In all the following questions, perform K-means clustering on the two input images (ppm and flower.png) for K = 3 clusters. Use only Euclidean distance as the distance measure for all iterations. Basic data units to be clustered are vectors containing pixel data, i.e., [r g b]. Perform 5 iterations of the algorithm. To visualize the output of k-means clustering, replace each pixels in the input image with the cluster center it belongs to and display the resulting image.

  <ul>

   <li>Perform K-means clustering with initial cluster means as follows:</li>

   <li><em>c<sup>init</sup></em><sub>1 </sub>– [255 0 0]</li>

   <li><em>c</em><em>init</em>2 – [0 0 0]</li>

   <li><em>c<sup>init</sup></em><sub>3 </sub>– [255 255 255]</li>

   <li>Perform K-means clustering on both images using random initialization of cluster means.Generate 3 random vectors of size 1×3 that are sampled from uniform distribution in [0 255] and use them as the cluster centers to begin the K-means with. Perform K-means clustering using <em>N </em>such initializations. The cost corresponding to the output of k-means clustering can be computed as</li>

  </ul></li>

</ol>

where <em>dist </em>measures the Euclidean distance between a pixel color value <em>p<sub>i </sub></em>and its cluster center <em>c<sub>k</sub></em>, and <em>P </em>refers to the total number of pixels in the image. Use N=30 (which means that you will repeat K-means clustering with 30 different random initializations), and find the cost corresponding to the output in each case. Among the 30 values that you got after repeatedly running the K-means, find the output corresponding to the lowest and highest value of C.

1

Comment on your observations.

<strong>Note:</strong>

<ul>

 <li>In this assignment, you will be working with a color image ‘car.ppm’.</li>

 <li>Each pixel in a color image has (R,G,B) components. The matrix containing color image data is a 3 dimensional matrix (e.g. – height*width*3). So [img(m,n,1) img(m,n,2) img(m,n,3)] will give the R,G,B components at (m,n) pixel respectively.</li>

 <li>At the end of K-means, if any cluster turned out to be empty, use only the non-empty clusters to display the image.</li>

 <li>People with Windows machines, please install Irfanview software in order to display .ppm</li>

</ul>

files.

–end–