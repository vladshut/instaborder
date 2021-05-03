# Instaborder

**Description**: Resizes an image and squares it up by padding and adding border for Instagram.

**Usage**: instaborder.sh [-h] [-q] [-v] [-f] [-r] [-s <size>] [-bs <bordersize>] [-c <color>] [-l <log_dir>] [-t <tmp_dir>] [-o <output>] <input>

Flags, options and parameters:

    -h|--help        : [flag] show usage [default: off]
    -q|--quiet       : [flag] no output [default: off]
    -v|--verbose     : [flag] output more [default: off]
    -f|--force       : [flag] do not ask for confirmation (always yes) [default: off]
    -r|--remove      : [flag] remove original [default: off]
    -s|--size <?>    : [option] size of the output image (default is the smae as original)
    -bs|--bordersize <?>: [option] size of the border  [default: 0 ]
    -c|--color <?>   : [option] color for the border   [default: white]
    -l|--log_dir <?> : [option] folder for log files   [default: /home/vs/log/instaborder]
    -t|--tmp_dir <?> : [option] folder for temp files  [default: /tmp/instaborder]
    -o|--output <?>  : [option] out file template (:ofolder: - original file folder, :oname: - original file name, :oext: - original file extension)  [default: :ofolder:/:oname:_squared.:oext:]
    <input>          : [parameter] input files (example: test/*.jpg)


## Example

**Command**
`./instaborder.sh -bs 100 -c lightgray  1.jpg`

---

**IN**
![1](https://user-images.githubusercontent.com/10393656/116870451-449a7600-ac1b-11eb-8769-c48d01f1d743.jpg)

---

**OUT**
![1_squared](https://user-images.githubusercontent.com/10393656/116870760-c7bbcc00-ac1b-11eb-9a95-130bcfa33d1d.jpg)

