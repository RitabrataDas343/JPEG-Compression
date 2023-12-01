# JPEG-Compression

JPEG (Joint Photographic Experts Group) is a popular image compression standard that achieves high compression ratios by applying a series of mathematical transformations on the image data. The JPEG encoder in this project takes a color/grayscale image as input and applies the following steps:

1. Divide the image into blocks.

2. Apply a discrete cosine transform (DCT) on each block to convert it into a frequency domain representation.

3. Quantize the DCT coefficients by dividing by the quantization matrix.

4. Perform zigzag scanning for each block.

5. Truncate each encode block to the specified number of coefficient parameters and return the encoded image

The JPEG decoder reverses the above steps to reconstruct the original image from the compressed data.

![Brown Pastel Flowchart Diagram Graph Template](https://user-images.githubusercontent.com/102947018/233417587-5d362e93-45d5-438d-add2-e1ed3a407128.png)

## Usage

- Requires Python 3.10+

- Install the required modules

    ```
    pip3 install -r requirements.txt
    ```

- Run the programs
    
    JPEG Compression

    ```
    python3 jpeg_compression.py
    ```

## Results

The algorithms were tested for a data set of color and grayscale images. 

Sample output:

![Figure_1](https://user-images.githubusercontent.com/102947018/233422987-fea9d017-6ce3-433e-840b-70ae185848fc.png)
