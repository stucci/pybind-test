[First steps — pybind11 documentation](https://pybind11.readthedocs.io/en/stable/basics.html#compiling-the-test-cases)

install
```shell
pip3 install pybind11
```

building binary module
```shell
c++ -O3 -Wall -shared -std=c++11 -fPIC $(python3 -m pybind11 --includes) example.cpp -o example$(python3-config --extension-suffix)
# -> example.cpython-36m-x86_64-linux-gnu.so
```

run
```shell
python3 main.py
```
