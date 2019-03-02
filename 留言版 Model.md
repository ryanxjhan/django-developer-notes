# 4.2 留言版 Model

## ORM
- 没有ORM的request
```python
def book_list(request):
  db = MySQLdb.connect(use='', db='', passwd='', host='localhost')
  cursor.execute('SELECT name FROM books ORDER by name')
  names = [row[0] for row in cursor.fetchall()]
  db.close()
```
1. 连接数据库
2. 连接cursor
3. 写query
4. 关闭数据库

> 能不能把表映射成类来处理？
> 只需要 `book.name`来获取数据?
> 
>答：可以，django的model就可以实现，让操作数据库就像类一样。

- ORM
`models.py`
```python
class UserMessage(models.Model):
  

```