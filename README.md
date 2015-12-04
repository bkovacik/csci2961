# csci2961 blog

## lab9
![](http://i.imgur.com/Kiy7nHV.png)
![](http://i.imgur.com/l6bZL77.png)
![](http://i.imgur.com/dc3FB7f.png)
![](http://i.imgur.com/tFfqOiL.png)

I decided I didn't want to build an entire community around my project, so I ended up joining the HabiticaOSS group. To my knowledge they haven't begun anything on their project either.

## lab7
1.
### Module

3 contributors

408708 lines of code

first 2e5c9debf819ed9d68fa6740cc548c1e10befa69

last 15238f0efadce295b594729d4146797ba8411516

### EveOnlineMarketAnalysisTool

6 contributors

344957 lines of code

first 90aa5d24e1d6e1fa171d4cd17bc1bd09b7924d83

last b92e13526e811df61b45fe6bee4452bddc5f4771

### LifeSim

5 contributors

212086 lines of code

first 4cbdf46ef6961aabebf32a015f3991c07f124498

last 735e0357e9db0fc1fcfac24d24a51aa4bb3ef7ae

### TrueVR

1 contributor

35 lines of code

first 874868628d87df69b3f6c4edef92a6a960e1470b

last c7f77c61a5dba6294095e37694e2575a3c94b8a9

### Trellis

1 contributor

3559 lines of code

first 26fd061eb84364e2811183b54f4f145c1177cb67

last f5f67398fa1cafa075b79b87f2ae2fb8c9090926

## Gitstats

For the most part, I want to say that Gitstats is more accurate. I don't actually know what the real stats were, but Gitstats tended to report a higher author/contributor count and a higher code count. In the case of TrueVR, the stats were identical, but this is probably because there was only a total of 35 lines of code.

I would assume that the leader in each of the projects is the one who made the initial commit.

## lab 5
1.
cmake .
```
-- The C compiler identification is GNU 4.9.1
-- The CXX compiler identification is GNU 4.9.1
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ethereal/Documents/csci2961/cmaketut/step1
```
make
```
Scanning dependencies of target Tutorial
[100%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o
Linking CXX executable Tutorial
[100%] Built target Tutorial
```
2.
cmake .
```
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ethereal/Documents/csci2961/cmaketut/step2
```
make
```
Scanning dependencies of target MathFunctions
[ 50%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o
Linking CXX static library libMathFunctions.a
[ 50%] Built target MathFunctions
Scanning dependencies of target Tutorial
[100%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o
Linking CXX executable Tutorial
[100%] Built target Tutorial
```
3.
cmake .
```
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ethereal/Documents/csci2961/cmaketut/step3
```
make
```
[ 50%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o
Linking CXX static library libMathFunctions.a
[ 50%] Built target MathFunctions
Scanning dependencies of target Tutorial
[100%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o
Linking CXX executable Tutorial
[100%] Built target Tutorial
```
ctest .
```
Test project /home/ethereal/Documents/csci2961/cmaketut/step3
    Start 1: TutorialRuns
1/5 Test #1: TutorialRuns .....................   Passed    0.03 sec
    Start 2: TutorialComp25
2/5 Test #2: TutorialComp25 ...................   Passed    0.03 sec
    Start 3: TutorialNegative
3/5 Test #3: TutorialNegative .................   Passed    0.02 sec
    Start 4: TutorialSmall
4/5 Test #4: TutorialSmall ....................   Passed    0.03 sec
    Start 5: TutorialUsage
5/5 Test #5: TutorialUsage ....................   Passed    0.04 sec

100% tests passed, 0 tests failed out of 5

Total Test time (real) =   0.19 sec
```
4.
cmake .
```
-- Looking for log
-- Looking for log - not found
-- Looking for exp
-- Looking for exp - not found
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ethereal/Documents/csci2961/cmaketut/step4
```
make
```
Scanning dependencies of target MathFunctions
[ 50%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o
Linking CXX static library libMathFunctions.a
[ 50%] Built target MathFunctions
Scanning dependencies of target Tutorial
[100%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o
Linking CXX executable Tutorial
[100%] Built target Tutorial
```
5.
cmake .
```
-- Looking for log
-- Looking for log - not found
-- Looking for exp
-- Looking for exp - not found
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ethereal/Documents/csci2961/cmaketut/step5
```
make
```
Scanning dependencies of target MakeTable
[ 25%] Building CXX object MathFunctions/CMakeFiles/MakeTable.dir/MakeTable.cxx.o
Linking CXX executable MakeTable
[ 25%] Built target MakeTable
[ 50%] Generating Table.h
Scanning dependencies of target MathFunctions
[ 75%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o
Linking CXX static library libMathFunctions.a
[ 75%] Built target MathFunctions
Scanning dependencies of target Tutorial
[100%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o
Linking CXX executable Tutorial
[100%] Built target Tutorial
```
./Tutorial 25
```
Computing sqrt of 25 to be 13
Computing sqrt of 25 to be 7.46154
Computing sqrt of 25 to be 5.40603
Computing sqrt of 25 to be 5.01525
Computing sqrt of 25 to be 5.00002
Computing sqrt of 25 to be 5
Computing sqrt of 25 to be 5
Computing sqrt of 25 to be 5
Computing sqrt of 25 to be 5
Computing sqrt of 25 to be 5
The square root of 25 is 5
```

## lab 4

I changed a line because it felt awkward to read.

It is important to maintain good documentation so that new or inexperienced users can attempt to solve problems that they encounter by themselves. This reduces the load on the developer themselves by reducing their need to provide steps to solve problems that could easily be placed in documentation.

Proprietary software is probably better for most users who specialize in a field that isn't computer science. They want out-of-the-box functionality and are willing to sacrifice customizability in order to get the job done. Often, proprietary software is offered in a bundle of some sort and guarantees that these pieces of software will work with each other, while open source might have to be mixed and matched to create a functional bundle. A company might be more inclined to something like this because it requires less setup and might have licensing that they need as a for-profit business.

Open source is better for rapid, crowd-sourced development. It is generally cheaper of cost and can be useful for those users who are willing to go the extra step to get the software working if needed. It might offer better technical help depending on the community that is responsible for its development as well. A personal user might be more inclined to use open source software because they can contribute back to its development and because licensing might not matter to them as much.

If I were starting a company, I'd want to use proprietary software for the reasons mentioned above. If I were doing a side project, I might still want to use proprietary software, depending on the application and the availability of an open source application that fulfills my needs. If not, then naturally I would use open source.

https://bugs.freebsd.org/bugzilla/show_bug.cgi?id=203338

## lab 3
### part 1

1. https://github.com/darkmeep/exercise01
4. ![](http://i.imgur.com/envtE1s.png)
    ![](http://i.imgur.com/bl0XcBg.png)

### part 2
4. ![](http://i.imgur.com/JHC0fwd.png)

### part 3
4. https://github.com/darkmeep/courseproject

## lab 2

1. done
2. Adding a license to your project adds a guarantee on the freedoms that your program offers. Depending on the restrictiveness of the license and whether the license is even open source or not, the program might offer more or less freedoms. In addition, if you don't add a license to your project, it defaults to the most restrictive license, ie one that offers no freedom to end users.
3. A project that has no licenses makes no guarantees about what it actually requires of the end user. For example, it might require compliance of the terms set forth by a software whose use isn't free. The license is also subject to retroactive changes that the user would have to agree to to continue using the software.
4. I agree that the Gopher project failed because of a lack of support. The open thinking did not apply to Gopher because it required some groups to pay for the service. While it was arguably a better service, it did not receive as much support as it needed because it was not an open system, which ultimately led to its failure.
5. The Sailfish OS most likely chose a non-Open Source license because it intends to create a meritocracy of developers such that not every developer can develop for the platform; only the ones that are good and serious.
6. Apache
7. done
8. done
9. I'd like to learn about the GLASS stack. We'd probably use the Apache license, as that is the license we chose for step 6.

## lab 1

1. done
2. done
3. done
4. Be direct.
    Give examples.
5. ![](http://i.imgur.com/5tQXiek.png)
6. ![](http://i.imgur.com/de7MKNW.png)
7. ![](http://i.imgur.com/vDcleuf.png)
8. ![](http://i.imgur.com/QaekLXF.png)
9. ![](http://i.imgur.com/H7CHwL4.png)
10. I started living off-campus this semester and I realized that a sort of "better grocery list" could be a worthwhile project. My roommate and I share the bill for necessities like food, but we both have a tendency to buy things that the other person might not want or need. Among other things, this improved grocery list could be used to write down which are actual necessities and which are luxuries that the individual roommate would pay for. Other features could be importing recipes into the list, priorities (is truffle butter *really* necessary). It would also contain rough estimates of pricing so a rough estimate of the grocery bill would be available. These prices could be inputted manually or in later versions, obtained via crowdsourcing or some other method.
