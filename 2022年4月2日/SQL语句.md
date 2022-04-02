# 关于sql语句的分类
sql语句有很多种，最好进行分类，这样更容易记忆，分为：
- DQL:数据查询语言(凡是带有select关键字的都是查询语句)
  - select ...
- DML:数据操作语言(凡是对表当中的数据进行增删改的都是DML)
  - insert：增
  - delete：删
  - updata：改
- DDL:数据定义语言(凡是带有create、drop、alter关键字的都是DDL)DDL主要操作的是表的结构，不是表中的数据。
  - create:新建，等同于增
  - alter:修改
  - drop:删除
- TCL:事务控制语言
  - 事务提交:commit
  - 事务回滚:rollback
- DCL:数据控制语言
  - 授权：grant
  - 撤销权限：revoke...
- 查看表中的数据
  - select * from 表名;

# 导入一下提前准备好的数据
- 如何将sql文件中的数据导入？
  - mysql> source F:\database_temp\bjpowernode.sql
- 不看表的数据只看表的结构
  - desc 表名;
