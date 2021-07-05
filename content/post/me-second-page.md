---
title: "Me Second Page"
date: 2021-07-05T14:53:41+05:00
draft: false
---
LOGO
==============
First we built the stack. It is useful because it return the data every time function completes and also returns the control. We reserved 16kb of memeory for the stack. ESP regster is used as stack pointer to give the address. To switch to 64 bit we used Long mode for which the code is written in the file.

Then we checked for multiboot, cpu-id,long-mode and error code. Linking btw virtual and physical address helped us to remove the memory loset issue. This process is known as paging in which we added page-tables in the previous main file.

Then, we added another file in src known as main64.asm ehich now contain 64 bits instead of 32 bits. We started long-mode labels. In these labels we passed 0 to all data registers so that they can function properly now.

After all these setups, I started writing the C code to print NUST on the screen. We built main.c file and kernel-main fnction is given the link in main6r also.

In Kernel we have three functions: Printclear to clear the screen. Setcolor to set background and front color. PrintStr to write some characters or text.

In print.h, we defined our printing interface.
Then we printed NUST LOGO given to you in image.
