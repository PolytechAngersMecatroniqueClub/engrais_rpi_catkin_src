# engrais_rpi_catkin_src
This folder should be named "src" and placed into the "~/catkin_ws/" folder.

# Remarks about the serial library:
It is from the following link : http://wjwwood.github.com/serial/, 
but all the "git" files has been removed in this already built version (rapsberry pi 3B+, xubuntu 18.04).

## Serial Library memo:

Serial Constructor:
```cpp
    Serial (const std::string &port="",
            uint32_t baudrate=9600,
            Timeout timeout=Timeout(),
            bytesize_t bytesize=eightbits,
            parity_t parity=parity_none,
            stopbits_t stopbits=stopbits_one,
            flowcontrol_t flowcontrol=flowcontrol_none)
```

parity_t structure:
```cpp
    enum serial::parity_t{
        parity_none = 0,
        parity_odd = 1,
        parity_even = 2
    }parity_t;
```
flowcontrol_t structure
```cpp
    enum serial::flowcontrol_t { 
        flowcontrol_none = 0,
        flowcontrol_software,
        flowcontrol_hardware
    }flowcontrol_t;
```

stopbits_t structure
```cpp
    enum serial::stopbits_t{
        stopbits_one = 1,
        stopbits_one_point_five,
        stopbits_two = 2
    }stopbits_t;
```
