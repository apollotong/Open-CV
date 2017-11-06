# Open_CV_601
Exercise one
How does a program read the cvMat object, in particular, what is the order of the pixel structure? 
Mat img = imread("image.jpg");
typedef struct CvMat
{
int type;
int step;
/* for internal use only /
int refcount;
int hdr_refcount;
union
{
uchar* ptr;
short* s;
int* i;
float* fl;
double* db;
} data;
