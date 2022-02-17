# raspberryPi_Setup


2022.02.17

- 현재 에러 : 버전불일치로 tensorflow 설치되지 않음.
라즈비안 64bit 설치 화면출력에서 error 
다시 라즈비안 32bit설치 진행

- bulid순서

1. python 설치 - tensorflow에 맞는
2. tensorflow 설치 - 중심으로 설치-> 신경써야하는 부분 (python버전/cpu-raspberry pi/32bit arm기반)
3. opencv 설치 - 파이썬 버전과 라즈베리파이 버전에 맞춰서 설치 


q-engineering 들어가서 
먼저 
1. tensorflow 설치
2. opencv 설치
T.F 2.2 
T.F 2.3
T.F 2.4


T.F 2.8?

우분투 설치12
https://ubuntu.com/download/raspberry-pi
설치하기전에 RAM확인 최소 4GB필요
cat /proc/meminfo 


처음버전체크 cat /etc/os-release
or uname -a
arch

파이썬 무슨 버전으로 깔아야하는지 확인해봐야한다







CPU 정보확인

// 전체 정보
cat /proc/cpuinfo

// 모델 정보
cat /proc/cpuinfo | grep 'model' | tail -1

// 물리 코어 수 정보
cat /proc/cpuinfo | grep 'processor' | wc -l
