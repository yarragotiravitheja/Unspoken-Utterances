# Unspoken Utterances LipNet Model

This repository contains the implementation of the Unspoken Utterances LipNet model, a deep learning architecture for lipreading.

## Model Architecture

The Unspoken Utterances model is implemented using the Keras Sequential API. Below is the summary of the model architecture:

```plaintext
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv3d (Conv3D)              (None, 75, 46, 140, 128)  3584      
_________________________________________________________________
activation (Activation)      (None, 75, 46, 140, 128)  0         
_________________________________________________________________
max_pooling3d (MaxPooling3D) (None, 75, 23, 70, 128)   0         
_________________________________________________________________
conv3d_1 (Conv3D)            (None, 75, 23, 70, 256)   884992    
_________________________________________________________________
activation_1 (Activation)    (None, 75, 23, 70, 256)   0         
_________________________________________________________________
max_pooling3d_1 (MaxPooling3)(None, 75, 11, 35, 256)   0         
_________________________________________________________________
conv3d_2 (Conv3D)            (None, 75, 11, 35, 75)    518475    
_________________________________________________________________
activation_2 (Activation)    (None, 75, 11, 35, 75)    0         
_________________________________________________________________
max_pooling3d_2 (MaxPooling3)(None, 75, 5, 17, 75)     0         
...
=================================================================
Total params: 8,471,924
Trainable params: 8,471,924
Non-trainable params: 0
'''
## Usage

To use the Unspoken Utterances LipNet model, follow these steps:

1. Clone the repository.
2. Install the necessary dependencies.
3. Load the pre-trained model weights.
4. Use the model for lipreading tasks.

## Downloading Data from GRID Corpus

To download data from the GRID corpus, visit [GRID Corpus](http://spandh.dcs.shef.ac.uk/gridcorpus/) and follow the provided instructions.

![Final Result]((https://github.com/yarragotiravitheja/Unspoken-Utterances/blob/main/output.png))


## Contributing

Contributions to improve the model or its documentation are welcome. Please fork the repository, make your changes, and submit a pull request.


## Acknowledgments

Special thanks to the authors of the original LipNet model for their pioneering work in the field of lipreading.
