# assignment2-Raavi
This is my Labcycle2 and this is repository 
# adithyakrishnaraavi
###### McDonalds near me is very good and spicy.
   I am living in the  maryville and i am living in the south main street which is near to the U.S Bank and this is a straight line and in this line we are having the theaters and other food plazas like BurgerKing and Tacos which is very near to that one and we are having the gas stations and motels around the corner.There are more good places than **Burger king** in this area particularly in college like  **Chick-fill-A**.

   ---

  ### Horizontal rule has been applied.
 Kansas international air port is located near to my food location.
  1.  step1 Start from Mcdonalds Maryville 64468.
  2.  step2 Drive fror 40 minutes on national highwat i-29.
  3.  step3 Fallow the instructions and stay on high way for 19 miles.
  4.  step4 And after 40 minutes you will encounter a kansas city and airport road diversions.
  5.  step5 Take diversiion and go to the airportroad and stay on it for 15 minutes.
  6.  step6  You will reach the destination as preceded.

  * Go to the McDonalds.
  * Check the Menu
  * Pick the items 
     * Veg and Non-veg.
     * Go to non-veg
     * Order the familypack spicy deluxe chicken burger with ranch.
[AboutMe](https://github.com/Adithyakrishna9/assignment2-Raavi/blob/main/AboutMe.md)

---

# SportsTable.
Below table repreents the Sports Activities that are being held in NWMSU and the event name is CATPAWS and the winner gets the BEARCAT title and the games in this event are cricket,BasketBall,Bdminton,Tennis and their locations respectfully StPeters,VolksCenter,Activity Arena CH123,Activity Arena CH216 and Additional costs for the Requirements that which are provided by college are gone cost  20,10,05,05 respectively.
 

|  SportsActivity      |       Location         | Additional costs for Requirements |
| -------------------- | ---------------------- | --------------------------------: |
| Cricket              | St Peters PT 213       |    20$ |
| BasketBall           | Volks Center VK 203    |    10$ |
| Badminton            | Activity Arena CH213   |    05$ |
| Tennis               | Activity Arena CH216   |    05$ |


---

# PithyQuotes
>    To improve is to change; to be perfect is to change often;
>>   *Winston Churchill*

>   Change Begins at the end of your comfort zone ;
>>   *Roy T.Bennett*
  True life is lived when tiny changes occur
   *Lee Telstey*
 
 ---

 # Algorithm Fetching Link

 > Graph traversal is a technique to visit the each nodes of a graph G. It is also use to calculate the order of vertices in traverse process. We visit all the nodes starting from one node which is connected to each other without going into loop.
  Lets go to the link <https://quescol.com/data-structure/graph-traversal-in-data-structure#:~:text=Graph%20traversal%20is%20a%20technique,other%20without%20going%20into%20loop.>

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
Source code Location <https://cp-algorithms.com/graph/breadth-first-search.html>

 >  In a graph, a vertex is called an articulation point if removing it and all the edges associated with it results in the increase of the number of connected components in the graph.
 >  An edge in an undirected connected graph is a bridge iff removing it disconnects the graph. For a disconnected undirected graph, definition is similar, a bridge is an edge removing which increases number of disconnected components.  
  Lets go the link for graphs  <https://www.geeksforgeeks.org/bridge-in-a-graph/>
  Lets go to the link bridges and articulation points <https://www.hackerearth.com/practice/algorithms/graphs/articulation-points-and-bridges/tutorial/>

  ```
  int n;
vector<int> g[MAXN] ;
bool used[MAXN] ;
vector<int> comp ;

void dfs(int v) {
    used[v] = true ;
    comp.push_back(v);
    for (size_t i = 0; i < (int) g[v].size(); ++i) {
        int to = g[v][i];
        if (!used[to])
            dfs(to);
    }
}
```

Source code Location <https://cp-algorithms.com/graph/search-for-connected-components.html>

  > In graph theory, the shortest path problem is the problem of finding a path between two vertices (or nodes) in a graph such that the sum of the weights of its constituent edges is minimized.
 Lets go to the Link<https://en.wikipedia.org/wiki/Shortest_path_problem#:~:text=In%20graph%20theory%2C%20the%20shortest,its%20constituent%20edges%20is%20minimized.>

 ```
 const int INF = 1000000000;
vector<vector<pair<int, int>>> adj;
void dijkstra(int s, vector<int> & d, vector<int> & p) {
    int n = adj.size();
    d.assign(n, INF);
    p.assign(n, -1);
    vector<bool> u(n, false);
    d[s] = 0;
    for (int i = 0; i < n; i++) {
        int v = -1;
        for (int j = 0; j < n; j++) {
            if (!u[j] && (v == -1 || d[j] < d[v]))
                v = j;
        }
        if (d[v] == INF)
            break;
        u[v] = true;
        for (auto edge : adj[v]) {
            int to = edge.first;
            int len = edge.second;
            if (d[v] + len < d[to]) {
                d[to] = d[v] + len;
                p[to] = v; }}}}
```
 SourceCode <https://cp-algorithms.com/graph/dijkstra.html>
 






