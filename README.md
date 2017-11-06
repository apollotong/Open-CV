# Open_CV_601
Exercise one<br>
-------------
How does a program read the cvMat object, in particular, what is the order of the pixel structure?<br>
typedef struct CvMat {<br>

int type;<br>
int step;<br>

int* refcount;<br>

union<br>
{<br>
    uchar* ptr;<br>
    short* s;<br>
    int* i;<br>
    float* fl;<br>
    double* db;<br>
} data;<br>

Exercise two<br>
----------------
		the values of the pixel at (20,25) in the RGB: 44 37 31
		the values of the pixel at (20,25) in the YCrCb: 38 132 124
		the values of the pixel at (20,25) in the HSV: 14 75 44

		For RGB, value ranges are all: 0-255
		For YCbCr, value ranges are: 16-235,16-240,16-240
		For HSV, value ranges are: 0-180,0-255,0-255
Exercise three<br>
----------------
