# LeetCode 203 - Remove Linked List Elements

## Problem Description

Given the head of a linked list and an integer `val`, remove all the nodes from the linked list whose value is equal to `val`.

Return the head of the modified linked list.

## Example

Input:

head = [1,2,6,3,4,5,6]
val = 6

After removing all nodes with value `6`:

Output:

[1,2,3,4,5]

## Approach

We use a dummy node before the actual head of the linked list.

The dummy node makes it easier to remove the first node if its value is equal to `val`.

We traverse the linked list using a pointer called `current`.

If the next node contains the given value, we skip that node by changing the `next` pointer.

Otherwise, we move `current` to the next node.

Finally, we return `dummy.next`, which is the head of the updated linked list.

## Algorithm

1. Create a dummy node and connect it to `head`.
2. Start traversing from the dummy node.
3. Check the value of the next node.
4. If it matches `val`, remove the next node.
5. Otherwise, move to the next node.
6. Continue until the end of the list.
7. Return the updated head.

## Time Complexity

**O(n)**

We visit each node of the linked list at most once.

## Space Complexity

**O(1)**

Only a few pointer variables are used, so no extra space proportional to the input size is required.

## Key Concepts

- Linked List
- Traversal
- Pointers
- Dummy Node
- Node Deletion

## Author

T.nandhini
