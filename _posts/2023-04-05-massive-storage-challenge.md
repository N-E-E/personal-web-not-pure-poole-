---
layout: post
title: 2022 Massive Storage Challenge(Design and Implementation of Data Retrieval Task Scheduling Algorithm)
date: 2023-04-05
last_modified_at: 2023-04-05
tags: [Engineer, Storage]
toc:  true
---


# Summary
Git Repo: https://github.com/N-E-E/2022-massive-storage-challenge

It's a wonderful experience! The team and I work together to solve a problem under the assitance of Prof. You Zhou. As for me, I do a lot of coding job to verify our ideas, and I enjoy the discussion.
Finlly we got a winning prize in the final competition(rank 10/74 in teams). Although it's not so excellent, considering most competitors are postgraduates, I think we've done good enough.

# Records for Code
### Update
11.7 Value Function Method Completed

11.8 Insight: Time Delay, Set Minimum Time, Only Process if Remaining Implementation Time is Below the Threshold (Effective, 226)

### Usage
```bash
cd src
python Demo.py
```

### Current Optimization Directions
Storage Method for Request Information: Heap/Tree/Lazy Deletion/Advanced Data Structures?
Priority Levels for Processing Various Requests: Urgency, Balancing Bonus/Penalty, Required Driver Space-----Comprehensive Consideration?
How to Select Requests to Fill Drives to Maximize Utilization at the Current Moment: Binary Search Optimization/Heuristic Algorithm?
Encapsulate a Scorer for Easy Maintenance in the Future. Haven't implemented penalty for sending requests to the wrong driver yet.
### File Structure
AlgCore: Contains core scheduling algorithms
AlgBase: Abstract base class (do not modify), unifies some API for algorithms (additional functions can be added in the inheriting class)
ListSeqAlg: Basic greedy scheduling implementation, relatively poor performance
loss_func_method_1: Value function method
xxx: Personally implemented algorithms can inherit AlgBase, placed under the AlgCore directory for easy access by Demo and Scheduler
logs: Output log folder
Scheduler: Officially provided interface; if implemented by inheriting AlgBase, just change self.method to your algorithm class for direct testing
score: Encapsulated simulated scorer
logger: Printing/Saving output results for debugging
Demo: Testing function; if implemented by inheriting AlgBase, no modification is needed.