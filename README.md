# GANs
### Building a DCGan from scratch1
**Generator** /n
  Blocks of /n
  * ConvTranspose2D
  * Batch normalization
  * Activations
**Discriminator**\n
  Blocks of \n
  * Conv
  * Leaky ReLU
  * Batch normalization
  * Fully connected layer
**Training**
  **  Train Discriminator ** \n
    * Feed real images and label them as real.
    * Feed generated images and label them as fake.
    * Update DD to minimize classification error.
**Train Generator**
  * Generate images and pass them to DD.
  * Update GG to maximize DD's error on generated images (i.e., fool DD).

Alternate between training discriminator and generator for each iteration.
  

