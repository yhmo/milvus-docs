这是因为 Milvus 在进行搜索时会将新生成的索引文件加载到内存，由于加载的索引文件和用于生成索引文件的原始向量文件总和小于 <code>cache.cache_size</code> 的上限，原始向量数据暂未被系统从内存释放。