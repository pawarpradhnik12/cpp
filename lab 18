#include <iostream>
#include <queue>
#include <stack>
#include <vector>

using namespace std;

class Graph {
private:
    int vertices;
    vector<vector<int>> adjacencyMatrix;

public:
    Graph(int v) : vertices(v), adjacencyMatrix(v, vector<int>(v, 0)) {}

    // Function to add an edge to the graph
    void addEdge(int from, int to) {
        adjacencyMatrix[from][to] = 1;
        adjacencyMatrix[to][from] = 1; // Uncomment if the graph is undirected
    }

    // Function for Breadth-First Search (BFS) traversal
    void BFS(int start) {
        vector<bool> visited(vertices, false);
        queue<int> q;

        visited[start] = true;
        q.push(start);

        while (!q.empty()) {
            int current = q.front();
            cout << current << " ";
            q.pop();

            for (int i = 0; i < vertices; ++i) {
                if (adjacencyMatrix[current][i] == 1 && !visited[i]) {
                    visited[i] = true;
                    q.push(i);
                }
            }
        }
        cout << endl;
    }

    // Function for Depth-First Search (DFS) traversal
    void DFS(int start) {
        vector<bool> visited(vertices, false);
        stack<int> s;

        visited[start] = true;
        s.push(start);

        while (!s.empty()) {
            int current = s.top();
            cout << current << " ";
            s.pop();

            for (int i = 0; i < vertices; ++i) {
                if (adjacencyMatrix[current][i] == 1 && !visited[i]) {
                    visited[i] = true;
                    s.push(i);
                }
            }
        }
        cout << endl;
    }

    // Function to convert from adjacency matrix to adjacency list
    vector<vector<int>> convertToAdjacencyList() {
        vector<vector<int>> adjacencyList(vertices);

        for (int i = 0; i < vertices; ++i) {
            for (int j = 0; j < vertices; ++j) {
                if (adjacencyMatrix[i][j] == 1) {
                    adjacencyList[i].push_back(j);
                }
            }
        }

        return adjacencyList;
    }

    // Function to convert from adjacency list to adjacency matrix
    vector<vector<int>> convertToAdjacencyMatrix(const vector<vector<int>>& adjacencyList) {
        vector<vector<int>> matrix(vertices, vector<int>(vertices, 0));

        for (int i = 0; i < vertices; ++i) {
            for (int j : adjacencyList[i]) {
                matrix[i][j] = 1;
            }
        }

        return matrix;
    }
};

int main() {
    Graph g(6);

    g.addEdge(0, 1);
    g.addEdge(0, 2);
    g.addEdge(1, 3);
    g.addEdge(1, 4);
    g.addEdge(2, 4);
    g.addEdge(3, 5);
    g.addEdge(4, 5);

    cout << "BFS Traversal: ";
    g.BFS(0);

    cout << "DFS Traversal: ";
    g.DFS(0);

    // Convert from adjacency matrix to adjacency list
    vector<vector<int>> adjacencyList = g.convertToAdjacencyList();
    cout << "Adjacency List:" << endl;
    for (int i = 0; i < adjacencyList.size(); ++i) {
        cout << i << ": ";
        for (int j : adjacencyList[i]) {
            cout << j << " ";
        }
        cout << endl;
    }

    // Convert from adjacency list to adjacency matrix
    vector<vector<int>> adjacencyMatrix = g.convertToAdjacencyMatrix(adjacencyList);
    cout << "Adjacency Matrix:" << endl;
    for (const auto& row : adjacencyMatrix) {
        for (int value : row) {
            cout << value << " ";
        }
        cout << endl;
    }

    return 0;
}
