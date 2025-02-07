---
title: Bubble sort 
author: Nikky Leone
date: 2022-09-09 20:55:00 +0800
categories: [Year 8, Algorithms]
tags: [bubble sort]
---

**A bubble sort algorithm goes through a list of data a number of times, comparing two items that are side by side to see which is out of order. It will keep going through the list of data until all the data is sorted into order. Each time the algorithm goes through the list it is called a ‘pass’.**

# Example

Imagine that you have a list of people who you want to sort by age, from youngest to oldest. A bubble sort can do this.

The list of ages is:

- 41, 15, 17, 32, 18, 28, 77 and 54

## First pass

The highlighted numbers are the numbers that are being compared.

- 41, 15, 17, 32, 18, 28, 77, 54

This is the list before it is sorted.

- 41, 15, 17, 32, 18, 28, 77, 54

The first two numbers are compared. 15 is smaller than 41 so they switch places.

- 15, 41, 17, 32, 18, 28, 77, 54

The next two numbers are compared. 17 is smaller than 41 so they switch places.

- 15, 17, 41, 32, 18, 28, 77, 54

The next two numbers are compared. 32 is smaller than 41 so they switch places.

- 15, 17, 32, 41, 18, 28, 77, 54

The next two numbers are compared. 18 is smaller than 41 so they switch places.

- 15, 17, 32, 18, 41, 28, 77, 54

The next two numbers are compared. 28 is smaller than 41 so they switch places.

- 15, 17, 32, 18, 28, 41, 77, 54

The next two numbers are compared. 41 is smaller than 77 so no change occurs.

- 15, 17, 32, 18, 28, 41, 77, 54

The next two numbers are compared. 54 is smaller than 77 so they switch places.

- 15, 17, 32, 18, 28, 41, 54, 77

This is what the list looks like after the first pass.

**The list is now more ordered than it was originally, but it isn’t yet fully in order of youngest to oldest. The list needs to go through another pass to compare the numbers again, so it can be sorted further.**

## Second pass

- 15, 17, 32, 18, 28, 41, 54, 77

This is what the list looks like after the first pass.

- 15, 17, 32, 18, 28, 41, 54, 77

The first two numbers are compared. 15 is smaller than 17 so no change occurs.

- 15, 17, 32, 18, 28, 41, 54, 77

The next two numbers are compared. 17 is smaller than 32 so no change occurs.

- 15, 17, 32, 18 28, 41, 54, 77

The next two numbers are compared. 18 is smaller than 32 so they switch places.

- 15, 17, 18, 32, 28, 41, 54, 77

The next two numbers are compared. 28 is smaller than 32 so they switch places.

- 15, 17, 18, 28, 32, 41, 54, 77

The next two numbers are compared. 32 is smaller than 41 so no change occurs.

- 15, 17, 18, 28, 32, 41, 54, 77

The next two numbers are compared. 41 is smaller than 54 so no change occurs.

- 15, 17, 18, 28, 32, 41, 54, 77

The next two numbers are compared. 54 is smaller than 77 so no change occurs.

- 15, 17, 18, 28, 32, 41, 54, 77

This is what the list looks like after the second pass.

**The set of data is now in order from youngest to oldest, but the algorithm does not know this yet as it made some changes in the second pass. The algorithm will only recognise that the list is in order if it makes no changes in a pass. The algorithm therefore needs to run for a third pass to compare the numbers again. As no changes will be made, the algorithm will then recognise that the data is in order.**

> If the data being sorted is a large set of data, it may take several passes to get the data sorted. 
{: .prompt-tip }
