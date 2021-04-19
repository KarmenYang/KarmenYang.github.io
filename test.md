```c++
#include<bits/stdc++.h>
using namespace std;
class Solution {
public:
    int removeElement(vector<int>& nums, int val) {
    	int i,j,n = nums.size();
    	for(i = 0 ,j = 0; i < n ; i++){
    		if(nums[i] == val)	continue;
    		nums[j++] = nums[i]; 
    	}
    	for(i = n - 1 ; i >= j ; i--){
    		nums.pop_back();
    	}
    	return j;
    }
};
int main(){
	std::vector<int> v;
	v.push_back(3);
	v.push_back(2);
	v.push_back(2);
	v.push_back(3);
	Solution c;
	int ans = c.removeElement(v,3);
	printf("%d\n",ans);
	for(int i = 0 ; i < v.size() ; i++)
		printf("%d\n",v[i]);
	return 0;
}
```

# 