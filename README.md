# StanfordExtra
12k labelled instances of dogs in-the-wild with 2D keypoint and segmentations. 

Dataset released with our ECCV 2020 paper: *Who Left the Dogs Out? 3D Animal Reconstruction with Expectation Maximization in the Loop*.

- [Project page](https://sites.google.com/view/wldo/home)
- [Paper](https://arxiv.org/abs/2007.11110)

![](splash.png)

## Usage
To understand how the dataset can be used, please read `demo.ipynb`.

## Installation
- All annotations, segmentations and metadata are sourced in a single .json file for ease of download. However, you will also need to download the [Stanford Dogs Dataset](http://vision.stanford.edu/aditya86/ImageNetDogs/) dataset to access the raw images. 

- For segmentation decoding, install `pycocotools`

`python -m pip install "git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI"`

- The `demo.ipynb` code is trivial to adapt to work with the full StanfordExtra dataset, by editing the line

```
img_dir = "sample_imgs" # Edit this to the location of the extracted tar file (e.g. /.../Images).
```

## Download & Versioning
The latest version of StanfordExtra is available for download within this repo. To view all released versions, view the [archive](https://drive.google.com/drive/folders/1MvN4hX2cdy0pMv0iUnL_UkobSYxZ0gzg?usp=sharing).

- Version 1.0 [23/08/20] - Initial release for ECCV 2020, 12k instances
- Version 0.1 [13/08/20] - Beta release, 11k instances

## Comments
You may also find the other datasets useful for your animal work:
- [Animal Pose Dataset](https://sites.google.com/view/animal-pose/)
- [RGBD-Dog Dataset](https://github.com/CAMERA-Bath/RGBD-Dog)
- [BADJA](https://github.com/benjiebob/BADJA)

We are also delighted to hear about your animal related activities! Please do visit [Benjamin Biggs](http://www.biggs.ai) to get in touch.

## Acknowledgements

If you make sure use of this annotation dataset, please cite the following paper:

```
@inproceedings{biggs2020wldo,
  title={{W}ho left the dogs out: {3D} animal reconstruction with expectation maximization in the loop},
  author={Biggs, Benjamin and Boyne, Oliver and Charles, James and Fitzgibbon, Andrew and Cipolla, Roberto},
  booktitle={ECCV},
  year={2020}
}
```

and the [Stanford Dog Dataset](http://vision.stanford.edu/aditya86/ImageNetDogs/) from which the images are derived:

```
@inproceedings{KhoslaYaoJayadevaprakashFeiFei_FGVC2011,
  author = "Aditya Khosla and Nityananda Jayadevaprakash and Bangpeng Yao and Li Fei-Fei",
  title = "Novel Dataset for Fine-Grained Image Categorization",
  booktitle = "First Workshop on Fine-Grained Visual Categorization, IEEE Conference on Computer Vision and Pattern Recognition",
  year = "2011",
  month = "June",
  address = "Colorado Springs, CO",
}
```

## Licensing
(c) Benjamin Biggs, Oliver Boyne, James Charles, Andrew Fitzgibbon and Roberto Cipolla. Department of Engineering, University of Cambridge 2020

By downloading this dataset, you agree to the [Creative Commons Attribution-NonCommercial 4.0 International license](https://creativecommons.org/licenses/by-nc-sa/4.0/). This license allows users to use, share and adapt the dataset, so long as credit is given to the authors (e.g. by citation) and the dataset is not used for any commercial purposes.

THIS SOFTWARE AND ANNOTATIONS ARE PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

