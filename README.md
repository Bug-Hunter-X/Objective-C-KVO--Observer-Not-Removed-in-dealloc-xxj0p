# Objective-C KVO: Observer Not Removed in dealloc

This repository demonstrates a common and subtle bug in Objective-C related to Key-Value Observing (KVO).  The issue occurs when an observer is added to an object but not properly removed, leading to potential crashes after the observed object is deallocated. 

The `bug.m` file shows the incorrect code where the observer is not removed in the `dealloc` method. The `bugSolution.m` file provides the corrected code with proper observer removal.

This is a classic example of a memory management issue that can be difficult to track down. Understanding how to properly manage KVO observers is crucial for writing robust and stable Objective-C applications.