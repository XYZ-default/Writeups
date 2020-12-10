# Extract M3 (Forensics - 300)

Firstly, followed the TCP Stream…

I found jpg header. 

So I thought that I need to export data from stream 0 to 20…

![picture](https://user-images.githubusercontent.com/65752885/101836910-9c511b80-3b6c-11eb-854a-115adca746a1.PNG)

![picture](https://user-images.githubusercontent.com/65752885/101836936-a96e0a80-3b6c-11eb-9b4f-b28eb781fe48.PNG)

I knew that I shouldn’t export data in ASCII. 

So, I changed ASCII to RAW…

And saved to a notepad…

And then, copied all hex values and opened with HxD…


![picture](https://user-images.githubusercontent.com/65752885/101836968-b4c13600-3b6c-11eb-8777-330612e1122b.PNG)

It starts with jpg header so I searched jpg footer ‘FF D9’…

![picture](https://user-images.githubusercontent.com/65752885/101837019-cb678d00-3b6c-11eb-88ff-98514b43c5b2.PNG)

And continuously found out that there is zip header after  jpg footer…

So, I separated two files and saved with related extensions…

I got jpg file and zip file that contain flag.pdf…

Firstly, I checked jpg file but I got nothing…

So, I cracked zip file password in kali…

![picture](https://user-images.githubusercontent.com/65752885/101837055-dae6d600-3b6c-11eb-8d74-b1d9d9e9614b.PNG)

I got zip password and extracted flag.pdf file…

When I opened flag.pdf file but there is nothing I can see…

![picture](https://user-images.githubusercontent.com/65752885/101837079-e508d480-3b6c-11eb-859c-4e6f7350cda2.PNG)

So, I pressed Ctrl+A to select all the content…

And I pasted to notepad…

![picture](https://user-images.githubusercontent.com/65752885/101837104-edf9a600-3b6c-11eb-8017-ed3f43786d58.PNG)

Finally, I got the flag…

*Flag: **shaktictf{h0p3_y0u_ar3_enj0ying_thi5}***
