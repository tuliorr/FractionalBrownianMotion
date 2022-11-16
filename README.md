# Fractional Brownian motion: Approximation by spectral synthesis

## 1. Intro
 
* This repository contains the Fractional Brownian motion in one and two dimensions represented by The spectral synthesis method (also known as the Fourier filtering method) for generating fBm.

* Brownian motion in one variable constitutes the simplest random fractal, and also it is at the heart of all the following generalizations. Small particles of solid matter suspended in a liquid can be seen under a microscope to move about in an irregular and erratic way. This was observed by the botanist R. Brown around 1827. The modeling of this movement is one of the great topics of statistical mechanics. Occasionally Brownian motion is also referred to as "brown noise". In one dimension we obtain a random process $X(t)$ , i.e. a function $X$ of a real variable $t$ (time) whose values are random variables $X(t_l)$, $X(t_2)$, etc.

## 2. Fractional Brownian motion in one-dimensional: ```fBm1d```

    Compute the one-dimensional fractal motion using Fourier filtering method.
   
    This function generate a fractal Brownian motion by spectral representation
    of random functions, this technique is known as spectral synthesis or 
    Fourier filtering method.
    
    The fractal Brownian motion is obtained from real part of fast inverse 
    Fourier transform in one-dimensional of Fourier coefficient.


    Parameters
    ----------
    L : int
        Lenght of array.
    H : float
        Hurst exponent which determines fractal dimension (0 < H < 1).
       
    Returns
    -------
    output : float ndarray
        Real part of Fast inverse Fourier transform in 1 dimension of Fourier coefficient
        
## 3. Fractional Brownian motion in two-dimensional: ```fBm2d```

    Compute the two-dimensional fractal motion using Fourier filtering method.
   
    This function generate a fractal Brownian motion by spectral representation
    of random functions, this technique is known as spectral synthesis or 
    Fourier filtering method.
    
    The fractal Brownian motion is obtained from real part of fast inverse 
    Fourier transform in two-dimensional of Fourier coefficient.
            
    Parameters
    ----------
    L : int
        Lenght of array along one dimension.
    H : float
        Hurst exponent which determines fractal dimension (0 < H < 1).
       
    Returns
    -------
    output : float ndarray
        Real part of Fast inverse Fourier transform in 2 dimensions of Fourier coefficient

## 4. Main

* ```main.py``` imports the two functions (fBm1d and fBm2d) and creates two arrays with lenght = 32 and Hurst exponent = 0.75 from a random seed with seed = 42


Source: The Science of Fractal Images, edited by H. Peitgen and D. Saupe (Springer, New York, 1988).
