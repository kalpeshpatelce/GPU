# Install GPU on Ubuntu 22.04
## First Find the Which GPU Card installed in your PCs
```
sudo lshw -c display
```
![image](https://github.com/kalpeshpatelce/GPU/assets/13175900/0f7049a7-3226-46a6-97ab-32694d26c922)

## Next, run the following command to list available drivers for your Nvidia card from the default Ubuntu repository. that recommended appropriate Driver
```
ubuntu-drivers devices
```
![image](https://github.com/kalpeshpatelce/GPU/assets/13175900/02fbfef2-1ba4-4c74-b56c-441938fb71a5)

## As you can see, it recommended driver for my GV100GL [Tesla V100 PCIe 32GB] card 
Now i run Appropriate command 
```
apt install nvidia-driver-550
```
![image](https://github.com/kalpeshpatelce/GPU/assets/13175900/48138360-7a1c-4265-a2fc-7bfac2fe6d29)

## After installation Verify the Driver installed or not
```
nvidia-smi
```
![image](https://github.com/kalpeshpatelce/GPU/assets/13175900/85094139-263e-4531-96a1-a621b7bedfcc)


# Method - 2
Get Driver from Nvidia Site
```
https://www.nvidia.com/download/driverresults.aspx/124722/en-us/
```
Download .run file and run into Ubuntu 22.04
