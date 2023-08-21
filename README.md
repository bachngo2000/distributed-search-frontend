# Distributed Search

## Walkthroughs

### Starting Apache ZooKeeper:
<img src=zookeeper_walkthrough.gif title='Video Walkthrough' width='' alt='Video Walkthrough' />

### Initializing the frontend server:

Since the search cluster coordinator and worker nodes have not been started, the search query returns no results

<img src=frontend_walkthrough.gif title='Video Walkthrough' width='' alt='Video Walkthrough' />

### Starting the search cluster coordinator and worker node:

<img src=final_walkthrough.gif title='Video Walkthrough' width='' alt='Video Walkthrough' />

As we can see, the leader (coordinator) node started on Port 8080, and the worker nodes are on Ports 8081, 8082, and 8083.

When we enter a search query, the coordinator communicates and delegates tasks to the worker nodes, which all run in parallel. Killing one or more worker nodes does not shut down or negatively impact the operations of the distributed system.

## Implementations of the Worker Nodes and Search Cluster Coordinator

To look at backend of the application, where the Worker Nodes and Search Cluster Coordinator are implemented, please visit: https://github.com/bachngo2000/distributed-search
