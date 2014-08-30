#C++ STL 使用总结
##map
- 头文件
```
#include <map>
```

- 定义
```
// 为什么不需要new map<string, int>()?
map<string, int> my_Map;
```

- 插入数据
```
my_Map["a"] = 1;
my_Map.insert(pair<string,int>("c",3));
my_Map.insert(make_pair<string,int>("d",4)); 
```

- 查找和修改数据
```
(1)	// 对于value类型为int，如果未找到，返回0
	// 如果判断被查找的数据是否存在？
	int i = my_Map["a"]; 
	my_Map["a"] = i;      
   
(2)	// my_Itr->first是key，my_Itr->second是value
	map<string, int>::iterator my_Itr; 
	my_Itr = my_Map.find("b");
	if (my_Itr != my_Map.end()) {
		int j = my_Itr->second;
	} 
```

- 删除数据
```
my_Map.erase("c");
my_Map.erase(my_Itr);
```

- 迭代数据
```
for (my_Itr=my_Map.begin(); my_Itr!=my_Map.end(); ++my_Itr)
{}
```

- 其他方法
```
my_Map.size()
my_Map.empty()
my_Map.clear()
```
