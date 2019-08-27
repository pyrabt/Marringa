### About Me
I grew up in central Wisconsin **GO PACK** and moved to Utah about 3 1/2 years ago. I'm currently in my final semester of my [Master's Degree in Software Development](https://msd.utah.edu/) at the University of Utah. I enjoy writing lower level programs in C++/C and most recently Rust. I love modal text editing, skiing, cycling, and learning new things.

### Why do I have a work history as a Lab Scientist?
After earning my Bachelor's Degree in Biotechnology, I committed 11 months to getting certified by the ASCP as a Medical Laboratory Scientist. I worked in clinical laboratories for the past 4 years, where my attention to detail and calmness in a stressful evironment made me a great team member. About 2 years ago I found myself hitting a "knowledge ceiling" in my field, so with nothing new to satisfy my keeness for learning I turned to my other interest, Computer Science. 

I am currently on my final semester class before I will receive a Masters of Software Development. I hope to apply the unique skills I have developed in the medical laboratory field to the challenges that await on your development team.

## Projects

## m(sd)alloc

### What it does
Just like the C Standard Library function malloc, my program allocates memory in page-sized chunks based on the passed bytes-to-allocate parameter.

### Purpose of this project
Learn how memory is managed and reserved within C/C++ programs.

### The implementation
Similar to how *std::malloc* operates under the hood, I used the system calls *mmap* and *munmap* to allocate/deallocate the memory. I implemented my own hashtable that store the *void pointer* address of each allocation using a simple hash function. Load factor was routinely calculated to ensure a low likelyhood of collisions when using a linear probing strategy.

[mmap/munmap usage](https://github.com/pyrabt/m-sd-alloc/blob/master/msdAlloc.cpp)

[hashtable caching](https://github.com/pyrabt/m-sd-alloc/blob/master/allocHashtable.cpp)

## JAVA DNS Resolver

### What it does
This is a local domain name server which fields dig requests, and then supplies answers via local cache results or pulls the answer from Google's DNS (8.8.8.8)

### Purpose of this project
Gain a better understanding of how the UDP message protocol works

### The implementation
Used Java's Datagram Socket/Message library to handle message transaction between dig and Google. All message formulation and parsing was performed via bit manipulation and the use of bytestreams. The trickiest part, and reason why static methods were used, was the refactoring and handling of compressed messages from Google's DNS.

![gif of running server](DNS.gif)

