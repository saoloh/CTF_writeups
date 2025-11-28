- you have a log file that is huge
- when you `cat` the file it returns garbage 
- so we suspict it is base64 we try to decode it 
> cat file.log | base64 -d 
- then we use the file command to know what type the file is 
> file file.log
- it is an image so we save it as an image
> cat file.log | base64 -d  > ing.png
- when you open the image there will be text inside it `base64` decode it it gives you the flag

