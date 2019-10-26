# NS2-for-Windows
A simple and easy port of the popular Network Simulator NS2 for the windows platform (no cygwin/virtualbox needed)

# Downloading

Download ```.zip``` or use ```git```

```git
git clone https://github.com/nimishbongale/NS2-for-Windows.git
```

Unzip the zipped file in your preferred directory.

## Installation

1. Install [chocolatey](https://chocolatey.org/)

Chocolatey takes care of your environment variables and all the nuances when it comes to installing new software which require some specific paths to executables to be present as home variables. 

This step may take a couple of minutes.

2. Run CMD prompt as administrator (system/32) once the installation is complete. Run the following command to install gawk (GNU awk). 

```cmd
choco install gawk
```
3. Navigate(```cd```) to the necessary directory where you have this repository cloned/unzipped.

## Testing 

Run 

```cmd
ns helloworld.tcl
```

If all your setup has been done perfectly, you should get the following output: 

```cmd
NS2-for-Windows>ns helloworld.tcl
Hello World - TCL
Hello World - AWK
```

The NSWireless animator window should also pop up.


## Usage

1. Write your tcl and awk files in the same directory where you have your ```ns.exe``` file. Alternatively, you could set an environment variable with the path to the ```ns.exe``` file. 

2. Run ns command with the your tcl file as parameter.

Sample Output: 
```cmd
NS2-for-Windows>ns sample.tcl
No. of packets dropped=6
```
If you are writing into a nam file,and the namtrace-all command has been levied in the tcl file, then you will also generate the nam file. 

3. In the window that pops up, select the tcl file by clicking on the ellipsis (```...```). Click on load.
4. In the bottom tab navigation, click on Simulation. 
5. Select the tr file by clicking on the ellipsis (```...```). Click on load. 

After some buffering, the animation should start playing. For adavnced features of NSWireless, visit [https://www.scribd.com/document/216718904/Ns2-Visual-Trace-Analyzer-Manual](https://www.scribd.com/document/216718904/Ns2-Visual-Trace-Analyzer-Manual)

Graphs showing network health and activites can also be plotted using this software.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html)
