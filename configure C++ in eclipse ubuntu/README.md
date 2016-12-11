Getting eclipse C++ ready in ubuntu
-----------------------------------

1. download cdt from their official website
2. set location of workspace
3. make susre you have gcc/g++ installed otherwise you can install by

```bash
sudo apt-get install gcc
sudo apt-get install g++
```
4. Open eclipse>preference>new C++ project>performed toolchains tab>executable folder>empty project> on right Toolchains select linux gcc>click make toolchains preferred

![MY_COOL_IMAGE](raw/master/img1.png)

<see img1.png>

5. Now create a new c++ project, create a source folder, create a file name it <something>.cpp
6. Now if this is the first time this project is created before running you need to build all
7. Now after building you have created the binary files. Now every time you change something in your file you just ctrl+F11

<see img2.png and img3.png>



