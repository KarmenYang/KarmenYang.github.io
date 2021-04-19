## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/KarmenYang/KarmenYang.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/KarmenYang/KarmenYang.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.


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
