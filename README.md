# NachOS
2017 Farn Wang OS

### Set-Up

1. Get ready with a 32 bit Liunx environment on Virtual Machine. Here we use ubuntu 14.04 (32bit).
2. Download the Nachos package and the cross compiler package from [course](http://cc.ee.ntu.edu.tw/~farn/courses/OS/OS2017/index.htm#line.project1).
```
wget http://cc.ee.ntu.edu.tw/~farn/courses/OS/OS2017/projects/project.1/mips-x86.linux-xgcc.tar.gz
wgat http://cc.ee.ntu.edu.tw/~farn/courses/OS/OS2017/projects/project.1/nachos-4.0.tar.gz
```
3. Untar file
`tar –zxvf nachos-4.0.tar.gz`
move cross compiler to the root
```
sudo mv mips-x86.linux-xgcc.tar.gz /
tar –zxvf /mips-x86.linux-xgcc.tar.gz
```
4. Set up the dependency
```
sudo apt-get install csh
sudo apt-get install g++
```
5. Build
`make`

### Error
Due to the dependency, it occur an error when we `make` the test part. It shows that we still missing a dependency which is `/usr/local/nachos`. To solve this follow steps below.

1. Download this repository either `git clone` or download zip is fine2. Go to `nachos` folder and move folder with `sudo`
```
cd ./NachOS-master/usr/local
sudo mv ./nachos /usr/local/
```
2. Re-build again
Make sure go back to previous `nachos-4.0/code` folder.
