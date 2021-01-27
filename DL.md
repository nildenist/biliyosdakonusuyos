<h3> 
Question  #1: Let's say we have lots of images(n) which a single image is 100 by 100 pixels. And we want to classify our images according to a business rule.
</h3>

**a)** How many features do we have?

</div>

<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

A single image has 100 * 100 = 10 000 features.
We have n images so the features that we have will be **n x 10 000**
 

</div>
</details>



**b)** Which neural network topology do you use for this classification problem and why? 

</div>

<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

CNN(Convolutional neural network).
Because is a special kind of FFNN(Feed-forward neural network) that significantly reduces the number of parameters in a deep naural network with many units without losing the quality of the model. <br/>

</div>
</details>


**c)** Think about a sky image. It is expected to pixels be close to one another and represents same type of information. How would you train your neural network to recognize regions of the same information of that sky image?
</div>

<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

Training neural network to recognize ***regions of the same information*** as well as the edges. This knowledge would allow the neural networks to predict the object represented in the image. <br/>
If the neural network detected multiple skin as regions and edges that look lika parts of an oval with skin-like tone on the inside and bluish tone on the outside, it's a face on the sky background. <br/>

</div>
</details>


**d)** We then split the image into square patches using a moving window approach. Which model does CNN use for this patches and what does this model need to learn? <br/> 
And how does this model behave in our sky image?
</div>

<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

CNN uses small regression models, each model receives a square patch as input. The goal of these small models is to learn to detect a specific pattern in the input patch. <br/>
In the sky image, one of the small regression model will learn to deteck the sky, another one will learn to detect grass, the third one will detect human face and so on.

</div>
</details>


**e)** If we want to get a large output matrix which properties of the convolution we should use?
</div>

<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

***Padding*** allows getting a larger output matrix, it's a width of the square of additional cells with which you surround the image before convolving it with the filter. <br/>
The cells added by padding usually contains zeros. If **padding=0** it means that no additional cells are added to image.

</div>
</details>

