qt creator 에서  OpenCV연동하기 (window에서)

환경 : VS2017  OpenCV3.4 CMake3.10.2 QTCreator4.5 MinGW5.3

-일단 기본 과정
http://iam777.tistory.com/419

-error참고

1.http://refrin.tistory.com/1

2.http://answers.opencv.org/question/168538/building-opencv-with-mingw-gcc-710-and-cmake-390-windresexe-unknown-option-w/

3.프로젝트를 만들때 MinGW 32bit선택

4.debug run 실행하면 'during startup program exited with code 0xc0000135' 에러 발생
-> 왼쪽메뉴 Projects -> Build & Run 에서 Run 선택 후 Run Environment에서 Path에 opencv dll 파일경로를 추가

-opencv library 추가
INCLUDEPATH += C:\\opencv-3.4\\newBuild\\install\\include
              C:\\opencv-3.4\\newBuild\\install\\include\\opencv

LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_calib3d340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_core340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_dnn340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_features2d340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_flann340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_highgui340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_imgcodecs340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_imgproc340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_ml340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_objdetect340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_photo340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_shape340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_stitching340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_superres340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_video340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_videoio340.dll
LIBS += C:\\opencv-3.4\\newBuild\\install\\x86\\mingw\\bin\\libopencv_videostab340.dll
