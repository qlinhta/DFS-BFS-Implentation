## DFS-BFS-Implentation

###DFS Algorithm

      DFS(G,v)   ( v is the vertex where the search starts )
         Stack S := {};   ( start with an empty stack )
         for each vertex u, set visited[u] := false;
         push S, v;
         while (S is not empty) do
            u := pop S;
            if (not visited[u]) then
               visited[u] := true;
               for each unvisited neighbour w of u
                  push S, w;
            end if
         end while
      END DFS()
            
###BFS Algorithm

    BFS (G, s)
      let Q be queue.
      Q.enqueue( s ) 
      mark s as visited.
      while ( Q is not empty)
           v  =  Q.dequeue( )

          //processing all the neighbours of v  
          for all neighbours w of v in Graph G
               if w is not visited 
                        Q.enqueue( w )         
                        mark w as visited.
