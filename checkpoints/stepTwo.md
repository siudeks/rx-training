
# Step 2

Create testable strategy for watching changes in visited tree structure. Use WatchService from jdk.
Use integration test with files and jimfs as file system.
Include observed changes in the reactive stream.
Include integration tests. Remember to observe changes recursively.
<br /><br />

**Tips**<br />
In terms of stream you need understand: Host Streams and other types, Stream Termination, Ways to merge streams,
Thread management, Observer contract (also agreement about thread safety), ConnectableObservable.