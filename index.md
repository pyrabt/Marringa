### About Me
I grew up in central Wisconsin **GO PACK** and moved to Utah about 3 1/2 years ago. I'm currently in my final semester of my [Master's Degree in Software Development](https://msd.utah.edu/) at the University of Utah. I enjoy writing lower level programs in C++/C and most recently Rust. I love modal text editing, learning new things, skiing, and cycling.

### Why do you have a work history as a Lab Scientist?
After earning my Bachelor's Degree in Biotechnology, I committed 11 months to getting certified by the ASCP as a Medical Laboratory Scientist. I worked in clinical laboratories for the past 4 years, where my attention to detail and calmness in a stressful evironment made me a great team member. About 2 years ago I found myself hitting a "knowledge ceiling" in my field, so with nothing new to satisfy my keeness for learning I turned to my other interest, Computer Science. With a constant cycle of new releases, and interesting things to master I found developing my own projects to be really satisfying. That inspired to me to apply for my current program where I have continued to master new skills and create interesting things.

## Projects

### JAVA DNS Resolver

## What it does
This is a local domain name server which fields dig requests, and then supplies answers via local cache results or pulls the answer from Google's DNS (8.8.8.8)

### Purpose of this project
Gain a better understanding of how the UDP message protocol works

### The implementation
Used Java's Datagram Socket/Message library to handle message transaction between dig and Google. All message formulation and parsing was performed via bit manipulation and the use of bytestreams. The trickiest part, and reason why static methods were used, was the refactoring and handling of compressed messages from Google's DNS.

![gif of running server](DNS.gif)

