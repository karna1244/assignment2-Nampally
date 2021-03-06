# assignment2-Nampally
# Karunakar Nampally
###### My favourite place is GOA
Goa is a **land that redefines holidays**, with its exquisite mix of sun, surf, and beaches; Goa has become the ultimate tourist destination. 

-----
# Directions for travelling from Maryville to Goa
1. Book a cab from maryville to kansas airport
2. Book flight through online
   1. Collect the boarding pass
   2. Wait for flight 
   3. Board the Flight
3. Complete your check-out process in Hyderabad

* Clothes
  * Sweatshirt
  * Shoes
* Cosmetics
  * Perfume
  * Body lotions
* Cash
* Snacks
  * French Fries
  * Cookies

[AboutMe](https://github.com/karna1244/assignment2-Nampally/blob/main/AboutMe.md)

# Table

Table with best foods in Marryville.

| Foods  |   Location    | Price |
|   ---  |   ---         |  ---  |
| Nuggets|   Harvey      |  $5   |
| Pizza  |   PizzaHut    |  $6   |
| Tuna   |   Walmart     |  $7   |

-----
# My favourite Quotes
>"Not giving a F is so key."-by 
*Mark Mason*<br>
> "No pain, No gain." -by
*Jane Fonda*

-----
## Code Fencing (Graph traversal)
In computer science, graph traversal (also known as graph search) refers to the process of visiting (checking and/or updating) each vertex in a graph. Such traversals are classified by the order in which the vertices are visited. Tree traversal is a special case of graph traversal.<https://en.wikipedia.org/wiki/Graph_traversal>

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```
<https://cp-algorithms.com/graph/breadth-first-search.html>
