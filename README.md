# Plant Disease Detection (GrowersBrainsML)

## Problem Definition

The user to be able to take a picture of their plant **leaf** and have detecting any possible disease from that.


![Graph](./images/graph.png)
 
 # About the Code & Implementation
 
 ## Data  
 The [Dataset](https://www.kaggle.com/vipoooool/new-plant-diseases-dataset) has over 38 Different Classes and 87k RGB image. And Below if my implementation - 
   - Used Color Images ( 3 Channel )
   - No Data Argumentation 
   - Data Notmalisation
   - Batch Size = 100
   - Training 90%, Validation 10%
 
## Model
The model is Resnet 18 ([Paper](https://arxiv.org/abs/1512.03385)). 

## Training 

With Training the model for 1 epoch, took 16 minutes in single Tesla P100 GPU (I use Kaggle Kernel ), with accuracy as metrics

- Training Loss = 0.118667
- Validation Loss = 0.066453
- Accuracy = 0.977258



# Tools we are using

- [FastAI](https://www.fast.ai/)  - For Data Reading & Preprocessing & Training DL Model
- [FastAPI](https://fastapi.tiangolo.com/) - For wrapping the DL Model into an API an send it to Backend Team
