## Commands and utilities to check the system resource capacity (on mac)
### Disk Space
As I use mac I use command ```df -h``` to check the current available disk space. It prints out the hard device and its parameters including available disk space. In my case I have 201Gi

<img width="572" alt="Screen Shot 2023-07-08 at 18 38 54" src="https://github.com/FK12344321/labs/assets/69464701/609d8f32-bece-4b8b-b551-274520a11e07">

### INodes
I use the same command with -i option ```df -i```. To find out the number of inodes (in total) I sum up the number of free and used inodes. In my case I have 2112947974 inodes

<img width="644" alt="Screen Shot 2023-07-08 at 18 43 05" src="https://github.com/FK12344321/labs/assets/69464701/baafdd43-c9bd-46c4-8e27-0a9fe6af20dd">

### Resource Consumption

To identify the process consuming the most RAM and CPU I use ```top``` command. As you can see this is systemstats process and it consumes 82% of cpu and 70M+ of memory (RAM)
<img width="734" alt="Screen Shot 2023-07-08 at 18 48 52" src="https://github.com/FK12344321/labs/assets/69464701/2111bb81-0874-46a4-b2ec-d674907e3fd3">


