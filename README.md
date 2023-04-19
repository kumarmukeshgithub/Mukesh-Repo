# Mukesh-Repo
      Array Program
      
1. Index of first repeating element in an array:


from collections import Counter

class Solution:
    #Function to return the position of the first repeating element.
    def firstRepeated(self,arr, n):
        
        #arr : given array
        #n : size of the array
    
        d=Counter(arr)
        for key,val in enumerate(arr):
            if d[val]>1:
                return key+1
        return -1
        #{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    t=int(input())
    for _ in range(t):
        n=int(input())
        
        arr=[int(x) for x in input().strip().split()]
        ob = Solution()
        print(ob.firstRepeated(arr, n))
# } Driver Code Ends
    
