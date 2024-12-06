# Very, very fast uiautomator (Android) conversion from XML to CSV

## Compile the app

### Linux/Windows examples

### GCC 
```g++-12 -std=c++2a -O3 uiautomatornolimit.cpp```

### ZIG 
```zig c++ -std=c++2a -O3 -g0 uiautomatornolimit.cpp```

## Run it 

### shell 

```sh 
uiautomatornolimit "C:\basjx\uiautomator_dump_to_csv\huge_example_dump.txt"
```
### python 
```py
import subprocess

exefile = r"C:\basjx\uiautomator_dump_to_csv\uiautomatornolimit.exe"
uidumpfile = r"C:\basjx\uiautomator_dump_to_csv\huge_example_dump.txt"

p = subprocess.run([exefile, uidumpfile], capture_output=True)

# In [2]: %timeit p = subprocess.run([exefile, uidumpfile], capture_output=True)
# 28.9 ms ± 301 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
```

