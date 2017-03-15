# UnixTools
一些处理数据的Unix小工具，支持管道操作。


借鉴awk的去重思想，当文本内容比较大的时候速度上比使用awk ‘!a[$0]++’快1倍，内存也差不多节约一倍左右。属于unix管道工具，接受标准输入，输出标准输出。按行去重，默认hashtable size是

#define HASH_TABLE_MAX_SIZE (1 << 27)
大家可以自行修改。
