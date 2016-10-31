**1. Clone wallet sources**

```
git clone https://github.com/BEASTLICK-INTERNET-POLICY-COMMISSION/bipcoinwallet.git
```


**2. Create git submoduleat the same level as `src`. For example:**

```
git submodule add https://github.com/BEASTLICK-INTERNET-POLICY-COMMISSION/bipcoin.git cryptonote
git submodule update --init -- "cryptonote"
```

**4 (Linux). Build**

```
mkdir build && cd build && cmake .. && make
```

**4 (Windows). Build**

Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, Boost 1.55, Qt 5.7. You may download them from:
http://www.microsoft.com/
http://www.cmake.org/
http://www.boost.org/
https://www.qt.io/

```
cmake -G "Visual Studio 12" -DCMAKE_PREFIX_PATH=C:\Qt\5.7\msvc2013
```
This will create a bipcoin.sln file which you can open in Visual Studio and build.
