## 1.Normalized Cross-Correlation(NCC)
### Describe:
Normalized Cross-Correlation is a robust method for measuring the similarity between two images. It is particularly useful for template matching and image alignment tasks.
### Formula:
  $NCC(I,T)=\frac{\sum_{x,y} (I(x,y) - \bar{I})(T(x,y) - \bar{T})}{\sqrt{\sum_{x,y} (I(x,y) - \bar{I})^2 \sum_{x,y} (T(x,y) - \bar{T})^2}}$<br>
where:<br>
* $I(x,y)$ is the pixel value of the input image at position $(x,y)$.
* $T(x,y)$ is the pixel value of the template image at position $(x,y)$.
* $\bar{I}$  and  $\bar{T}$  are the mean values of the input and template images, respectively.
### Link:
https://www.mathworks.com/help/images/ref/normxcorr2.html
## 2.Mutual Information(MI)
### Describe:
Mutual Information measures the amount of information that one image contains about another. It is effective for image registration tasks, especially when the images have different modalities.
### Formula:
$MI(I, J)$ = $\sum_{i,j} p_{IJ}(i,j) \log \frac{p_{IJ}(i,j)}{p_I(i)p_J(j)}$<br>
where:<br>
* $p_{IJ}(i,j)$  is the joint probability distribution of pixel values in images $I$  and  $J$ .
* $p_I(i)$  and  $p_J(j)$  are the marginal probability distributions of pixel values in images  $I$  and  $J$ , respectively.
### Link:
https://www.youtube.com/watch?app=desktop&v=eJIp_mgVLwE
## 3.Mean Squared Error (MSE) with a Shift-Invariant Component
### Describe:
Mean Squared Error can be adapted to be less sensitive to small shifts by incorporating a penalty for large differences in pixel values while tolerating minor misalignments.
### Formula:
$MSE(I,J)=\frac{1}{n} \sum_{x,y} \min \left( (I(x,y) - J(x,y))^2, \alpha \right)$<br>
where:<br>
*  $n$  is the number of pixels.
*  $\alpha$  is a threshold parameter that controls the sensitivity to large differences.

