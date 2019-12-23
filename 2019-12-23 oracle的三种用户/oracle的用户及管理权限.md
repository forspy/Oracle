oracle的三种用户

sys用户（超级管理员，可以创建数据库）：数据库中所有的数据字典表和视图都储存在sys模式中。sys用户主要用来维护信息系统和管理实例。
system用户（管理员，不能创建数据库）：system用户是默认的系统管理员、该用户拥有Cracle管理工具使用的内部表和视图。通常通过system用户管理数据库用户、权限和储存等

scott用户：scott用户是Oracle数据库的一个示范账户，在数据安装时创建。

登陆命令： sqlplus 用户名/密码 conn 用户名/密码
解锁用户(不行加;)：alter user 用户名 account unlock
锁定用户：alter user 用户名 account lock

修改用户密码：

a：conn / as sysdba
b:alter user 用户名 identified by 密码

显示当前登陆账户： show user;
退出命令：exit