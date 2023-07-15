## System information 
I used ```htop``` command to  display RAM, CPU,and network info separately. All I had to do wat to run the command and pick the options I wanted to display. 

Here I displayed CPU only: 

<img width="1197" alt="Screen Shot 2023-07-15 at 21 03 37" src="https://github.com/FK12344321/labs/assets/69464701/68022bae-fd2a-4fd1-93ec-3e8e525f371f">

Here is RAM: 
<img width="1162" alt="Screen Shot 2023-07-15 at 21 05 17" src="https://github.com/FK12344321/labs/assets/69464701/b6bdcc78-bcb1-478b-9a20-b7745118940e">

And network: 

<img width="330" alt="Screen Shot 2023-07-15 at 21 06 26" src="https://github.com/FK12344321/labs/assets/69464701/f9e95b88-8500-4a29-b0b9-5d7172ea2c6e">

And to display the specs I used the following commands:
- I used ```lscpu``` command to display the information about the processor (Also I used '''cat /proc/cpuinfo'''). Here is the result (number of cpu cores is correct)
<img width="740" alt="Screen Shot 2023-07-15 at 20 00 47" src="https://github.com/FK12344321/labs/assets/69464701/c508b42e-b46c-4bc8-8bc2-204eba286467">

- To display the RAM properties I used ```cat /proc/meminfo``` (We can see that the size of the memory is approximately equal to the parameter that I picked creating the VM)
<img width="346" alt="Screen Shot 2023-07-15 at 21 22 58" src="https://github.com/FK12344321/labs/assets/69464701/7aad2c8a-2c84-4aea-906f-c26023a99ed1">
  
- ```df -H``` can be used to display hard disk info or ```lsblk```
