* Multi source Shortest Path Algorithm
    See Algorithm
* Also helps in detecting negative cycles
  If after the algorithm, dist[i][i] < 0 -> it means there is a negative cycle
Intuition - 
Go Via every vertex/node
For example you want to go from 0 to 1
Then go from 0 to 2 and then from 2 to 1
Then go from 0 to 3 and then from 3 to 1 and so on


public:
	void shortest_distance(vector<vector<int>>&matrix){
	    // Code here
	    int n = matrix.size();
	    for(int i = 0; i<n; i++)
	    {
	        for(int j = 0; j<n; j++)
	        {
	            if(matrix[i][j] == -1)
	                matrix[i][j] = 1e9;
	        }
	    }
	    
	    for(int k = 0; k<n; k++)
	    {
	        for(int i = 0; i<n; i++)
	        {
	            for(int j = 0; j<n; j++)
	            {
	                matrix[i][j] = min(matrix[i][k] + matrix[k][j], matrix[i][j]);
	            }
	        }
	    }
	    
	    //To detect a negative cycle.
	    for(int i = 0; i<n; i++)
	    {
	        if(matrix[i][i] < 0)
	        {
	            cout << "There is a negative cycle"
	        }
	    }
	    
	    for(int i = 0; i<n; i++)
	    {
	        for(int j = 0; j<n; j++)
	        {
	            if(matrix[i][j] == 1e9)
	                matrix[i][j] = -1;
	        }
	    }
	}
