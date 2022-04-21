# Json_with_cpp
## install Json on visual studio c++
1- First download [This](https://github.com/open-source-parsers/jsoncpp) as zip<br /><br />
2- Extract it <br /><br />
3- Run file named "amalgamate.py"  (if nothing occure open file using any python compiler then run it)<br /><br />
4- Now you can see new folder created named "dist"<br /><br />
5- Copy dist , include folders and go to the project destination then paste (near to .cpp file)<br /><br />
6- Now open project properties with Visual studio -> at the top of the window make sure that Configuration set as (all configurations) and platform set as (all platforms) -> open C/C++ tab -> click on additional include directories and press edit then press 3 dots (...) and open project folder then choose include folder (near to dist and depug) -> press apply and Ok  <br /><br />
7- Open project destination -> open dist and copy .cpp file then past it on sorurce File on your compiler <br /><br />
8-  Open project destination -> open dist and  open json folder and copy 2 .h files then paste them on Header files on your compiler<br /><br />
7- Congratulations Your project is ready to use json <br /><br />

Code for testing : <br />
```cpp
#include<iostream>
#include<json\json.h>
using namespace std;
int main() {
	std::unique_ptr<std::string> httpData(new std::string());
	Json::Value jsonData;
	Json::Reader jsonReader;
	if (jsonReader.parse(*httpData.get(), jsonData))
	{
	}
}
```

## Write on files

## Read from files
