# stevensStringLib

Welcome to stevensStringLib! This is a simple C++ library full of convenient functions for working with strings. It was created to make C++ more accessible and read more like plain English.


## Demo
#### Separate a string:
```
std::string myString = "Charmander,Squirtle,Bulbasaur";

std::vector<std::string> myVector = separate( myString, "," );

for(int i=0; i < myVector.size(); i++)
{
  std::cout << myVector[i] << std::endl;
}
```
Output:
```
Charmander
Squirtle
Bulbasaur
```


## Requirements

C++ 17


## Easy Installation!

To get started, add the following to the top of your .cpp file:

`include "<insert path to the repo folder here>/stevensStringLib.h"`


Give the library namespace a short, catchy name:

`namespace strlib = stevensStringLib;`


And then you're good to go!

`std::vector<std::string> words = strlib::separate("Hello world!, " ");`


More changes and updates to come soon! Just establishing the github page as of now. Feel free to make any changes and make pull requests!

## Documentation

The documentation for this library is written to a series of offline webpages that can be viewed by clicking the "Open Documation" link in the `docs` folder. This documentation was generated by [Doxygen][4].

## Testing

stevensStringLib contains a suite of tests to validate its functionality within the `testing` folder. All testing is carried out with [Google Test][5].


To run these tests on your machine, you should use the cmake tool in the `testing` folder by running the command `cmake -S . -B ./build_of_test`.
This will generate an makefile to create an executable in the `testing/build_of_test` folder. Then, go to the `testing/build_of_test` folder and run the command `make`.
Once you have done this, you should have an executable named `test` in the `testing/build_of_test` folder which you can run the tests with.

## Benchmarking

stevensStringLib also contains benchmarking so you can see how fast and efficient its functions are in the `benchmarking` folder.

## Special Thanks

Julien Jorge for [his detailed code review][1]

[r/cpp][2] for their collective critiques and contributions

Rhymu for his [guide][3] on using CMake to link GoogleTest with a unit test program 



[1]: https://julien.jorge.st/posts/en/so-you-asked-for-feedback-stevensstringlib/

[2]: https://www.reddit.com/r/cpp/comments/18hlkgd/working_on_an_easytouse_c_string_library/

[3]: https://www.youtube.com/watch?v=Lp1ifh9TuFI

[4]: https://www.doxygen.nl/index.html

[5]: https://github.com/google/googletest