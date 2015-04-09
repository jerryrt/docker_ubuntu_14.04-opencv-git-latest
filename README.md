# docker_ubuntu_14.04-opencv-git-latest
Dockerfile to build the latest OpenCV(with python2, python3 and Java bindings support).

It is a faily big image(over 2.8GB in size at the moment), what it contains:

* A complete set of building tools needed to build OpenCV from source.
* OpenJDK7, Python2(2.7.4)and Python3(3.4).
* OpenCV bindings with all of the compoenents above. 

I am building this in order to ease the setup of my learning of OpenCV with different
languages, on different machines. 

Since OpenCV is a very fast moving project and its Python3 support is relatively new, 
building all from source codes is a natural choice for me here, instead of using old
pre-build binaries.

If you do want to try out with this image, you can type this(the image downloading could take a while :-( ):

`docker run jerrytian/ubuntu_14.04-opencv-git-latest python3.4 -c "import cv2; print(cv2.__version__);"`

Enjoy ;-)
