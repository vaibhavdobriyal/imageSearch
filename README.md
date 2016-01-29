# imageSearch
OpenCV Experiments - Image Processing - Computer Vision Examples

These are some of initial explorations of Open CV with Python.
Do read the blog post http://www.pyimagesearch.com/2014/12/01/complete-guide-building-image-search-engine-python-opencv/

<b>Environment Setup - MAC OSX Python PyCharm</b>

Configuring PyCharm to use Python and OpenCV on  MACOSX

The process requires creation of virtual environment - since there are multiple versions of Python installed on OSX. We recommend using brew to install python and not use the system one. Please don’t break the system one else the osx will run into issues.
							
$ brew doctor	
Follow any troubleshooting advice it gives.	 							Now, update Homebrew:							
$ brew update
Run the following command to install Python 2.7:					
$ brew install python
			
Now, we can install NumPy. Homebrew's selection of Python library packages is limited so we use a separate package management tool called pip, which comes with Homebrew's Python:
 $ pip install numpy
	
SciPy contains some Fortran code, so we need an appropriate compiler. We can use Homebrew to install the gfortran compiler:							
$ brew install gfortran									
$ pip install scipy
To install OpenCV on a 64-bit system (all new Mac hardware since late 2006), run:
 $ brew install opencv

Download Jet Brains PyCharm and set it up.

Create a project and then go to preferences for project and set up Virtual environment say python_devenv - point the python to /usr/bin/Cellar/ and where your python is. 

Next task is to create the syslinks for opencv. Go to the directory where homebrew installed opencv (/usr/local/Cellar/opencv/2.4.12_2/lib/python2.7/site-packages) and create following links

$ln -s cv.py ~/python_devenv/lib/python2.7/site-packages/cv.py
$ ln -s cv2.so ~/python_devenv/lib/python2.7/site-packages/cv2.so

You are good to go.




