# MSAI_531_A01
# A Study Guide in Sonnet Form

## Table of Contents

1.  Data Preprocessing: Normalization
2.  Generative Adversarial Networks (GANs)
    -   Components of Generator and Discriminator
    -   Loss Functions
    -   Training Process
3.  Variational Autoencoders (VAEs)
    -   Loss Functions
4.  Autoencoders
    -   Loss Function
5.  Mathematical Concepts
    -   Convolution
    -   Bias and Variance
    -   Optimization
6.  Gradient Descent
    -   Weight Update Rule
    -   Mean Squared Error (MSE)
7.  Conclusion

## Data Preprocessing: Normalization

Normalization doth scale input data bright,\
To standardized ranges, models do thrive,\
Equal contribution in learning’s flight,\
Thus stable performance, we’ll surely derive.

**Normalization Formula:**

$$
x_{\text{normalized}} = \frac{x_{\text{raw}}}{255}
$$

**Example:**\
If $x_{ ext{raw}} = 128$:

$$
x_{\text{normalized}} = \frac{128}{255} \approx 0.502
$$

## Generative Adversarial Networks (GANs)

GANs, a model of adversarial might,\
Two networks dance—a Generator bold,\
And Discriminator, with its keen insight,\
In zero-sum games, their tales are told.

### Components: Generator and Discriminator

**Generator (G):**\
Creates data from random noise,\
Its output, a $G(z)$ to rejoice.

**Discriminator (D):**\
Classifies as real or fake,\
Probability $D(x)$ it will stake.

### Loss Functions

For GANs, we quantify each’s strife,  

### Discriminator Loss ($L_D$):  
$$
L_D = -E_{x \sim p_{\text{data}}}[\log D(x)] - E_{z \sim p_z}[\log(1 - D(G(z)))]
$$

### Generator Loss ($L_G$):  
$$
L_G = -E_{z \sim p_z}[\log D(G(z))]
$$

## Training Process

In this process, we iteratively train,\
The Discriminator first, then the G,\
Improving each, amidst the data's gain,\
A game of wits, 'twixt D and G.

## Variational Autoencoders (VAEs)

VAEs, models of probabilistic grace,\
Learn latent structures, in data they hide,\
With Encoder and Decoder, they embrace,\
A normal distribution as their guide.

### Loss Functions

**Reconstruction Loss (**$L_{ ext{rec}}$):

$$
L_{\text{rec}} = \text{Binary Crossentropy}(x, \hat{x})
$$

**KL Divergence Loss (**$L_{K L}$):

$$
L_{KL} = -\frac{1}{2} \sum_{i=1}^{d} (1 + \log \sigma_i^2 - \mu_i^2 - \sigma_i^2)
$$

### Total VAE Loss ($L_{V A E}$)

$$
L_{V A E} = L_{\text{rec}} + L_{K L}
$$

## Autoencoders

These networks compress and reconstruct,\
With Encoder and Decoder in their scheme,\
Through MSE they measure what’s deducted,\
From input to output, a dream within a dream.

### Loss Function:

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (x_i - \hat{x}_i)^2
$$

## Mathematical Concepts

### Convolution

In neural nets, a method most fair,\
Filters slide, capturing patterns so rare.

### Bias and Variance

Errors that plague, we must understand,\
High bias doth underfit, while variance is grand.\
Thus in this realm of math and design,\
The learning unfolds, intricate and fine.

## Optimization

### Gradient Descent

To find the path where loss doth cease to grow,  
In gradient descent, we follow the flow.  
With step size bold, we traverse the steep,  
Adjusting our weights, the secrets we keep.

Let $\theta$ be the weight we strive to refine,  
With the gradient, we measure the line:

$$
\theta = \theta - \eta \nabla J(\theta)
$$

Here, $\eta$ represents the learning rate bright,  
Guiding us gently toward the optimal sight.

### Weight Update Rule

Each weight shall change by the gradient's decree,  
To minimize loss, as is plain to see.  
The update rule thus doth elegantly state:

$$
w_{\text{new}} = w_{\text{old}} - \eta \cdot \nabla L(w)
$$

Where $L$ be loss, our burden to bear,  
As we aim for precision with utmost care.

### Mean Squared Error (MSE)

To measure the error with clarity keen,  
The mean squared error provides a scene:

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$

Where $y_i$ are true values, and $\hat{y}_i$ are the guesses,  
A means to assess all our learning's stresses.

## Conclusion

Thus concludes our study of networks profound,\
In the realms of data, where insights abound.\
With knowledge of GANs, VAEs, and more,\
May your journey in learning forever soar.\
Embrace the formulas, let wisdom ignite,\
For in understanding, the future shines bright.
