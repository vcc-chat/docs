1.  new_object(self, name, id=None, bucket="file"):
    - 描述：创建新对象
    - 参数：
      - name(必填): 文件名称
      - id(可选): 文件id
      - bucket(可选): 桶名称
    - 返回值: [预签名url,文件id]

2.  new_object_with_content(self, name, content, bucket="file"):
    - 描述：创建带内容的新对象
    - 参数：
      - name(必填): 文件名称
      - content(必填): 文件内容
      - bucket(可选): 桶名称
    - 返回值: 文件id
3.  get_object(self, id, bucket="file"):
    - 描述：获取对象
    - 参数：
      - id(必填): 文件id
      - bucket(可选): 桶名称
    - 返回值: 预签名url 或 None
4.  has_object(self, id, bucket="file"):
    - 描述：检查是否存在对象
    - 参数：
      - id(必填): 文件id
      - bucket(可选): 桶名称
     - 返回值: 布尔值
5.  get_object_content(self, id, bucket="file"):
    - 描述：获取对象内容
    - 参数：
      - id(必填): 文件id
      - bucket(可选): 桶名称
    - 返回值: 对象内容
