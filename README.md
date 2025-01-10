# GANs
### Building a DCGan from scratch1
**Generator** \
  Blocks of
  * ConvTranspose2D
  * Batch normalization
  * Activations
**Discriminator** \
  Blocks of 
  * Conv
  * Leaky ReLU
  * Batch normalization
  * Fully connected layer
**Training** \
  **Discriminator** \
  * Feed real images and label them as real.
  * Feed generated images and label them as fake.
  * Update DD to minimize classification error.
**Generator**
  * Generate images and pass them to DD.
  * Update GG to maximize DD's error on generated images (i.e., fool DD).

Alternate between training discriminator and generator for each iteration.
  

