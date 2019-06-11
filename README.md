
# Counting proliferating cells in *Drosophila* midguts 

This code was made with the intent to be able to identify PH3+ cells in a 2D maximum intensity projection of *Drosophila* midguts. This program attempts to identify PH3+ cells by looking for bright, small, red dots.

A common problem I've noted that prevents effective use of an automated cell counter is that the *Drosophila* midgut cannot be dissected by itself. There are always other tissues with it that often have bright red puncta that is counted when it shouldn't be. To solve this problem, I have tried to develop a program that identifies puncta as well as determining if it's in the midgut or not based on structure.

## Getting Started

### Prerequisites

This code requires the following packages to run, with instructions on how to install if needed

**numpy**

`pip install numpy`

**Pillow PIL**

`pip install Pillow`

**skimage**

`pip install scikit-image`


**matplotlib**

`pip install matplotlib`


### How to run the demo set

* So you should just press go (?), as long as none of the files have been moved around since being unzipped. The cells need to be run in order for it to work.

* First cell loads in all the programs and sets up environment to get down to **B U S I N E S S** if any errors load make sure you have all the necessary packages listed in prerequs.

* Second cell is a plotting function that we will use later

* Third cell we start using the demo data. This will load in all the files in a directory, take their numpy arrays, and shove it all into a list containing your data that you can now play around with.

* After this, all the variables are the same, so all you need to do is refer to the index of the image you want in order to do all the functions on it.

`y = read_images("folder/")`

y is now a list of arrays

`y[9][:,:,1]` 

y [list index] [x,y, (RBG) ]

### Caution

* This tends to run for a long time and occasionally throws timeout errors

### Getting the size of the gut

* I tried and failed miserably at this...I think because I was trying to get edge detection to work? Could probably work with different types of stains (wg, 10xSTAT92E-GFP stain in bands along outside of gut)


```python

```
