#OSINT
## 
We look at the linkedin, inside the linkedin

![image3](https://github.com/Nupture/CTFWriteup/assets/39788429/31a09a44-1e5c-4d49-b6f0-ddb8d56dc8c3)

Inside the creadional part, we click on of the accreditation and it show a dogge picture.

![image2](https://github.com/Nupture/CTFWriteup/assets/39788429/5872ac31-8b02-4209-867c-32f4021dfdf0)

We notice that it is inside the imgur, so we decided to look at the comment section. 

![image8](https://github.com/Nupture/CTFWriteup/assets/39788429/53300749-9dba-479a-a03a-d09cadde698f)

There is a guy mention about the github who called rssianheker, so we think this is very SUS

![image6](https://github.com/Nupture/CTFWriteup/assets/39788429/b46b127d-9bc9-4b4b-9c1c-0af01b026cb6)

Found the github profile and we can see this, confidential which is sus, plus the commit connect is also sus.

![image1](https://github.com/Nupture/CTFWriteup/assets/39788429/ee0a5b17-3fa4-4d8f-b130-8574ff7fd5c2)


We found this, throw inside the cyber chef and ye we found the flag

![image5](https://github.com/Nupture/CTFWriteup/assets/39788429/50a1ddf1-b824-4c92-90b8-9b1e7ab95fc6)

Flag: RWSC{Russ14n_H4ck3r_D4b3st}

# Network 
## I Hope You Have The Software

Going through servers one by one…

![image4](https://github.com/Nupture/CTFWriteup/assets/39788429/b1aa55e3-0146-4fe9-947b-2b6087819a39)

After checking all the configs and settings of the servers in the logical view, we couldn’t find anything. 
We were thinking of throwing this challenge but then I decided to switch to the physical view for a last attempt. 
The first server i checked was server 6 and in the http service under the services tab we can see there’s a index.html file. 
Clicking on the edit allows us to view the content of the file and eventually the flag :)



Flag: RWSC{!t5_a_t4c3r_f!l3_:D}

