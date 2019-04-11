
# Step 1

Create testable algo to convert tree-based structure to iterable collection.
<br /><br />

**Tips**<br />
- Define the root of tree-based structure as kind of your custom Node interface with minimal functionality need by conversion algo.
Do not use any specific types like Path / File etc.

- Example of contract(interface):

```public interface Node<T> {
       @NotNull T getPayload();
       @NotNull Iterable<Node<T>> getChildren();
   }```