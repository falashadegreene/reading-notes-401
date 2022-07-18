# Big O Notation

Big O notation according to the article (A beginner's guide to Big O Notation) "Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm"

## O(1)

O(1) according to the reading is an algorithm that will always executes in the same time (or space) regardless of the size of the input data set.

`bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}`

## o(N)

O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.

example code:

`bool ContainsValue(IEnumerable<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true;
    }
    return false;
}`

## O(N²)

represents an algorithm whose performance is directly proportional to the square of the size of the input data set.

example code:

`bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++)
    {
        for (var inner = 0; inner < elements.Count; inner++)
        { 
            // Don't compare with self
            if (outer == inner) continue;
            if (elements[outer] == elements[inner]) return true;
        }
    }
    return false;
}`

## Logarithms

My understanding of Logarithms is it's the power to which a number must be raised in order to get some other number

## Names and Values in Python

- Names refer to values for example:
`x = 23
 print(x)`

- Names are reassigned independently

- Values live until no references

- Assignment never copies data

- Changes are visiable through all names
