# LinuxCmd 101

## Overview

Points : 10
Category : Bash

## Description

Each point is linked to another point, connect the link and win the Flag!

link : https://hubchallenges.s3-eu-west-1.amazonaws.com/Forensics/linux-chal.tar.gz  (Download This File)

## Solve

After Download This File 

First : Extract Him By Using : $ tar -xf linux-chal.tar.gz

Then Go To File By : $ cd linux-chal

Let's See What is Inside It : $ ls

It's a Folder Called (cat)

Let's Get In It To See : $ cd cat

Let's Show : $ ls

There Is a ZIP File ! ... Let's Extract Him : $ 7z x exec.zip

mmmmm ! It's Need a Password Then Let's See

Try This : $ ls -al

hmmm ! There is An Hidden File Let's See What is inside : $ cat .pass.txt

There is a Password : qwerty1245

Then Extract Him : $ 7z x exec.zip 

Yes ! 

$ cd exec
$ ls

There is Another ZIP File And Required a Password 

Let's Try This : $ cp - test 
$ chmod +x test
$ ./test

There is Password : 998877665544332211

After Extract : $ cd ascii

What! There is a 9 Files Let's Try This To Know What File Have Password : $ file *

f6 Is an ASCII Text 

Let's See : $ cat f6

Password is : rryuiytqpyuiqyofdkhsjhfewojnhfdss

Let's Extract size37.zip By This Password

Go To size37 : $ cd size37

See : $ ls

Then Search for File That Size Equal 37 : $ ls -al

The test5 Is 37 : $ cat test5

Password Is : 62094n902m2x-28mx4t9xy282y49ty9824yt

Let's Extract next.zip By Password 

$ cd next

There Is File Called : (nexttocybertalents) Let's See : $ cat nexttocybertalents

Oh no ! There Is Many Words....emmm Look at The Name Of file The Password Is Next To The (cybertalents) Word 

$ cat nexttocybertalents | grep cybertalents 

The Password is : orderby1337 To Extract (NumberOne.zip)

$ 7z x NumberOne.zip
$ cd NumberOne
$ ls

There File Called : decodeme1.zip

Let's Decode It : $ zip2john decodeme1.zip

Copy Hash and Put In file called (hash.txt) : $ nano hash.txt

Then Use This To decode : $ john --format=zip hash.txt --wordlist=One

The Password is : infrastructure

$ 7z x decodeme1.zip
$ cd decodeme1
$ ls

There Is File Called : (pass) Let's See : $ cat pass

Password is : (dXNlbWVhc3Bhc3N3b3Jk) in Hash Unknown Type

Go To : https://www.tunnelsup.com/hash-analyzer/  Type : base64

Go To : https://www.base64decode.org/  To Decode It : Output : usemeaspassword

$ 7z x decodeme2.zip
$ cd decodeme2
$ ls

There Is File Called : flag.txt Let's See : $ cat flag.txt

There Is Flag : synt{f1zcyr_yvahk_101} mmmm... But It Incorrect Let's Decode It 

Go To : https://rot13.com 

The Result Is : flag{s1mple_linux_101}
