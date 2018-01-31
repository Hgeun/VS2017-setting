qt creator 에서  OpenCV연동하기 (window에서)

환경 : VS2017  OpenCV3.4 CMake3.10.2 QTCreator4.5 MinGW5.3

-일단 기본 과정
http://iam777.tistory.com/419

-error참고

1.http://refrin.tistory.com/1

2.http://answers.opencv.org/question/168538/building-opencv-with-mingw-gcc-710-and-cmake-390-windresexe-unknown-option-w/

3.프로젝트를 만들때 MinGW 32bit선택

4.막 에러 debug run 실행하면 'during startup program exited with code 0xc0000135' 에러 발생
-> 왼쪽메뉴 Projects -> Build & Run 에서 Run 선택 후 Run Environment에서 Path에 opencv dll 파일경로를 추가
