
# OSINT
## Medellin Cartel
No clue at all before the hint, so let's look at the hint, we able to know:
- the sicarios - Blacky aka Nelson Hernandez
- uniten IG
- Dig inside the IG, metadata

We tried to look at the comment first, there are no people name Blacky or Nelson, but when we look at the "following"/follower, 

![Pasted image 20240306204109](https://github.com/Nupture/CTFWriteup/assets/39788429/b87a363e-fffc-44e5-b552-e2da76738207)

We able to find someone call exactly what we trying to find, look inside the profile, download the image and search for metadata but nothing found,

but when we inspect the image, we able to find the flag!

![Pasted image 20240306204247](https://github.com/Nupture/CTFWriteup/assets/39788429/b48e50bf-8e75-4cfc-b23e-f0837fc22285)

flag: RWSC{Bl4cky_S1c4r1o}

## Cali Cartel
The question mention about how the Cali Cartel fail, so after some search,
we lock on something who betrayal the Cartel, Jorge Salcedo,

![Pasted image 20240306205718](https://github.com/Nupture/CTFWriteup/assets/39788429/417d9726-8bac-4274-9734-b02494bbaf50)

here are the fun part coming up, search the name, apply the google-fu and that's it!

![Pasted image 20240306205521](https://github.com/Nupture/CTFWriteup/assets/39788429/a1a17c90-330f-4959-b275-bea6ebef58d6)

moral of the story, dont be the betrayer and don't skip your class, OSINT BASIC MY BABY
flag: RWSC{C4L1_C4RT3L_PWN3D}

# MISC 
## Hidden Discord
We have been invited into a discord server and mention that the flag are all inside the server.
This is a easy one as a discord geek, let's welcome our best friend, **Better Discord**

Voice text channel found the first part!

![Pasted image 20240306204636](https://github.com/Nupture/CTFWriteup/assets/39788429/69d762aa-7c15-4703-a779-9e986148816d)

1 pic with 2 part of flag! Part 2 and Part 4.

![Pasted image 20240306204606](https://github.com/Nupture/CTFWriteup/assets/39788429/1b484f54-ef5a-4099-8546-0fb7c79e0c4f)

the part 3 is inside the event!

![Pasted image 20240306204721](https://github.com/Nupture/CTFWriteup/assets/39788429/0f962e79-96b3-44c1-ada5-07577f066221)

the last part is the hard one, by following the hints on the channel name "dont tell others about profile pic", we get to know that the flag is inside the profile picture.

by download the server icon, it just 64px big, lmao

![Pasted image 20240306204913](https://github.com/Nupture/CTFWriteup/assets/39788429/454933ae-6b44-4881-8baa-6436bf5ae7ff)

by enlarge it, it's still blur but we able to read something and try to guess it

![Pasted image 20240306204936](https://github.com/Nupture/CTFWriteup/assets/39788429/2da2ed11-cb21-4d8d-b3ce-a0c6fde397d9)

flag: 1. RWSC{r34d_d15c0rd_d3v3l0p3r_API_r3f3r3nc3}

# SCADA
## Prison Break
This is the hard one, so we just look at the hint(only the part helps me),

- I suggest you to find documentation for the Prison Scada System. Just in case you dont know, most Ladder Logic file is like system_water.ld
- Didn't even need to learn plc to access it, just need to know its format and location
- [hints link](https://www.wired.com/images_blogs/threatlevel/2011/07/PLC-White-Paper_Newman_Rad_Strauchs_July22_2011.pdf "https://www.wired.com/images_blogs/threatlevel/2011/07/PLC-White-Paper_Newman_Rad_Strauchs_July22_2011.pdf")
- As mentioned, find the diagram name, then access to it in the website directory follow the format of ladder logic name (water_tank_valve.ld)

What can we know from here, 
- all the naming in ladder logic file are having (.id)
- no need to learn plc
- the link

We able to spot the name of this file = (peneumatic_prison_sliding_door)
![Pasted image 20240306211005](https://github.com/Nupture/CTFWriteup/assets/39788429/53081b3d-9047-4b01-b172-353961d0bc07)

That the first clue, compare with the hint's naming, we tried to put _ to replace the space, and (.id) after it 

Look nothing over here but if we scroll down, the flag is there!
![Pasted image 20240306211213](https://github.com/Nupture/CTFWriteup/assets/39788429/2462011d-0028-4510-9dca-40db06fb0899)

I guess is the time to learn ladder logic, meh
hints are so useful (OuO)b

FLAG: RWSC{107f9494d760061dc24c394030caf914}

# Cryptograph

## round and round

2126226{19122929121712_6121911821_26422_842928}

everything look similar for us, so we admit that it is alphabet like (1=A, 2=B)
but the number is too big that cannot fit inside 1-26

what are the flag format: RWSC! so we just put RWSC with 2126226,

we able to know that all the number are plus 3, so we can just minus it and apply the rule.

Bingo!

flag RWSC{PIZZINI_CIPHER_WAS_EAZY}

# Network

ok find password in cap file, what we gonna think first? Aircarck-ng
so we just throw it into aircarck-ng
![Pasted image 20240306213459](https://github.com/Nupture/CTFWriteup/assets/39788429/50528ed5-2a30-4148-9da6-6b1fe65ab680)

EZ!
flag: RWSC{anonymous}
