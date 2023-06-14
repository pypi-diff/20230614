# Comparing `tmp/tools_hjh-2.5.4.tar.gz` & `tmp/tools_hjh-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.5.4.tar", last modified: Fri Apr 14 11:41:59 2023, max compression
+gzip compressed data, was "dist\tools_hjh-2.5.5.tar", last modified: Wed Jun 14 01:43:47 2023, max compression
```

## Comparing `tools_hjh-2.5.4.tar` & `tools_hjh-2.5.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.4/LICENSE
--rw-rw-rw-   0        0        0      207 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-04-14 11:41:47.000000 tools_hjh-2.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/tools_hjh/
--rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.4/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9420 2023-04-13 09:26:36.000000 tools_hjh-2.5.4/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.4/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.4/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.4/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.4/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    33359 2023-04-14 11:39:10.000000 tools_hjh-2.5.4/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.4/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.4/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.4/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.4/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 01:43:47.000000 tools_hjh-2.5.5/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.5/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-06-14 01:43:47.000000 tools_hjh-2.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:43:47.000000 tools_hjh-2.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-06-14 01:43:16.000000 tools_hjh-2.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:43:46.000000 tools_hjh-2.5.5/tools_hjh/
+-rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.5/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9787 2023-06-08 01:39:35.000000 tools_hjh-2.5.5/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.5/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.5/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.5/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.5/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    41576 2023-06-08 02:48:19.000000 tools_hjh-2.5.5/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.5/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.5/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.5/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.5/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:43:47.000000 tools_hjh-2.5.5/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:43:44.000000 tools_hjh-2.5.5/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-06-14 01:43:44.000000 tools_hjh-2.5.5/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-06-14 01:43:44.000000 tools_hjh-2.5.5/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      453 2023-06-14 01:43:45.000000 tools_hjh-2.5.5/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 01:43:44.000000 tools_hjh-2.5.5/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.5.4/tools_hjh/Chrome.py` & `tools_hjh-2.5.5/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/DBConn.py` & `tools_hjh-2.5.5/tools_hjh/DBConn.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,26 @@
             return False
         else:
             return True
 
     def get_row(self):
         return self.row
     
+    def get_table(self, begin_num=1, end_num=None):
+        table = []
+        table.append(self.get_cols())
+        idx = 0
+        while self.next():
+            idx = idx + 1
+            if idx >= begin_num:
+                table.append(self.get_row())
+            if end_num != None and idx >= end_num:
+                break
+        return table
+    
     def close(self):
         try:
             self.cur.close()
         except:
             pass
         try:
             self.conn.close()
```

### Comparing `tools_hjh-2.5.4/tools_hjh/HTTPRequest.py` & `tools_hjh-2.5.5/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/HTTPTools.py` & `tools_hjh-2.5.5/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/Log.py` & `tools_hjh-2.5.5/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/MemoryDB.py` & `tools_hjh-2.5.5/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/OracleTools.py` & `tools_hjh-2.5.5/tools_hjh/OracleTools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding:utf-8
 from tools_hjh.DBConn import DBConn
-from tools_hjh.DBConn import QueryResults
 from tools_hjh.MemoryDB import MemoryDB
 from tools_hjh.Tools import line_merge_align, locatdate, merge_spaces, analysis_hosts, locattime
-
+from tools_hjh import Tools
+    
 
 def main():
     rows = []
     for idx in range(0, 10):
         row = (idx, idx, idx)
         rows.append(row)
     testDB = DBConn('sqlite', db='test.ora_conn')
@@ -100,15 +100,15 @@
                     || ' ' || descend
                 ) over(
                     partition by index_name 
                     order by column_position 
                     rows between unbounded preceding and unbounded following
                 ) index_str
                 , uniqueness, index_type
-                from t_idx 
+                from t_idx order by 2
             '''
             rss = mdb.db_conn.run(sql).get_rows(True)
             mdb.close()
             for rs in rss:
                 name = rs[0]
                 col = rs[1].lower()
                 if rs[3] == 'BITMAP':
@@ -137,15 +137,15 @@
                 where t.owner = ?
                 and t.table_name = ?
                 and t.owner = t2.owner
                 and t.constraint_name = t2.constraint_name
                 and t.table_name = t2.table_name
                 and t.constraint_type in('P','U')
             ) group by constraint_name, constraint_type
-            order by constraint_name, constraint_type
+            order by 3
         '''
         rss = ora_conn.run(sql, (username, table)).get_rows(True)
         for rs in rss:
             name = rs[0]
             c_type = rs[1]
             cols = rs[2].lower()
             if c_type == 'U':
@@ -167,15 +167,15 @@
         dst_username = dst_username.upper()
 
         src_desc = OracleTools.desc(src_conn, src_username, src_table_name)
         dst_desc = OracleTools.desc(dst_conn, dst_username, dst_table_name)
         mess = line_merge_align(str_1=src_username + '.' + src_table_name + '\n' + src_desc
                                        , str_2=dst_username + '.' + dst_table_name + '\n' + dst_desc
                                        , iscompare=True) + '\n\n'
-        return mess, src_desc == dst_desc
+        return mess, '\t*' not in mess
 
     @staticmethod
     def get_ddl(dba_conn, username, type_, obj_name):
         """得到某个对象的ddl语言"""
         username = username.upper()
         obj_name = obj_name.upper()
         type_ = type_.upper()
@@ -220,14 +220,177 @@
         ddl_sqls = ddl_sqls + '-- 注释' + '\n'
         for r in dba_conn.run(sql, (username, table)).get_rows(True):
             ddl_sqls = ddl_sqls + "comment on column " + username + "." + table + "." + r[0] + " is '" + r[1] + "';\n"
             
         return ddl_sqls    
     
     @staticmethod
+    def get_table_ddl_2(ora_conn, username, table, simple_mode=True):
+        """得到表结构，包括索引、约束和默认值情况"""
+        username = username.strip()
+        table = table.strip()
+        user_upper = username.upper()
+        table_upper = table.upper()
+        all_tablename_upper = user_upper + '.' + table_upper
+        username = username.upper()
+        table = table.upper()
+        
+        exists_sql = '''
+            select 1 from dba_tables 
+            where owner = ?
+            and table_name = ?
+        '''
+        rs = ora_conn.run(exists_sql, (username.upper(), table.upper())).get_rows()
+        if len(rs) == 0:
+            return '-- ' + all_tablename_upper + ' 不存在'
+        
+        mess = '-- drop table ' + all_tablename_upper + ' cascade constraints;\ncreate table ' + all_tablename_upper + '(test_col number);\n'
+        
+        # 列 类型 非空约束 默认值
+        sql = '''
+            select column_name, 
+                case 
+                    when data_type = 'VARCHAR2' or data_type = 'CHAR' then 
+                        data_type || '(' || data_length || ')'
+                    when data_type = 'NVARCHAR2' then 
+                        data_type || '(' || char_length || ')'
+                    when data_type = 'NUMBER' and data_precision > 0 and data_scale > 0 then 
+                        data_type || '(' || data_precision || ', ' || data_scale || ')'
+                    when data_type = 'NUMBER' and data_precision > 0 and data_scale = 0 then 
+                        data_type || '(' || data_precision || ')'
+                    when data_type = 'NUMBER' and data_precision = 0 and data_scale = 0 then 
+                        data_type
+                    else data_type 
+                end column_type, nullable, data_default
+            from dba_tab_cols where owner = ? and table_name = ? and column_name not like '%$%' order by column_id
+        '''
+        cols_ = ora_conn.run(sql, (username, table)).get_rows(True)
+        lenNum = 0
+        for col_ in cols_:
+            if lenNum < len(col_[0]):
+                lenNum = len(col_[0])
+        for col_ in cols_:
+            colstr = '"' + col_[0] + '"'
+            typestr = col_[1]
+            colstr = colstr + ' ' + typestr
+            if col_[2] == 'N':
+                nullable = ' not null'
+            else:
+                nullable = ''
+            if col_[3] != 'None':
+                data_default = ' default ' + col_[3].strip('\n')
+            else:
+                data_default = ''
+            mess = mess + 'alter table ' + all_tablename_upper + ' add ' + colstr.upper() + data_default + nullable + ';\n'
+        mess = mess + 'alter table ' + all_tablename_upper + ' drop column test_col' + ';\n'
+        # 约束 类型 列和列排序
+        sql = '''
+            select constraint_name, constraint_type
+            , max(cols)
+            from (
+                select t.constraint_name, t.constraint_type
+                , to_char(
+                    wm_concat(t2.column_name)
+                    over(partition by t.constraint_name order by t2.position)
+                ) cols
+                from dba_constraints t, dba_cons_columns t2
+                where t.owner = ?
+                and t.table_name = ?
+                and t.owner = t2.owner
+                and t.constraint_name = t2.constraint_name
+                and t.table_name = t2.table_name
+                and t.constraint_type in('P','U')
+            ) group by constraint_name, constraint_type
+            order by constraint_name, constraint_type
+        '''
+        rss = ora_conn.run(sql, (username, table)).get_rows(True)
+        constraint_name = []
+        for rs in rss:
+            name = rs[0]
+            c_type = rs[1]
+            cols = rs[2]
+            if c_type == 'U':
+                mess = mess + 'alter table ' + all_tablename_upper + ' add unique (' + cols + ')' + ';\n'
+            elif c_type == 'P':
+                mess = mess + 'alter table ' + all_tablename_upper + ' add primary key (' + cols + ')' + ';\n'
+            constraint_name.append(name.lower())
+        # 索引 类型 列和列排序
+        sql = '''
+            select t.index_name
+            , t.index_type
+            , t2.column_name
+            , t3.column_expression
+            , t2.descend
+            , t2.column_position
+            , t.uniqueness
+            from dba_indexes t, dba_ind_columns t2, dba_ind_expressions t3
+            where t.table_owner = ? 
+            and t.table_name = ? 
+            and t.owner = t2.index_owner
+            and t.table_owner = t2.table_owner
+            and t.index_name = t2.index_name
+            and t.table_name = t2.table_name
+            and t2.index_owner = t3.index_owner(+)
+            and t2.table_owner = t3.table_owner(+)
+            and t2.index_name = t3.index_name(+)
+            and t2.table_name = t3.table_name(+)
+            and t2.column_position = t3.column_position(+)
+            order by t.index_type, t2.column_position
+        '''
+        qrs = ora_conn.run(sql, (username, table))
+        rows = qrs.get_rows()
+        col = qrs.get_cols(True)
+        if len(rows) > 0:
+            mdb = MemoryDB()
+            mdb.set('t_idx', col, rows)
+            # 降序索引也体现为函数索引，列名会用"col_name"，而字符串用'str'
+            sql = '''
+                select distinct index_name
+                , group_concat(
+                    replace(case when column_name like 'SYS_%$' then column_expression else column_name end, '"', '')
+                    || ' ' || descend
+                ) over(
+                    partition by index_name 
+                    order by column_position 
+                    rows between unbounded preceding and unbounded following
+                ) index_str
+                , uniqueness, index_type
+                from t_idx 
+            '''
+            rss = mdb.db_conn.run(sql).get_rows(True)
+            mdb.close()
+            for rs in rss:
+                name = rs[0]
+                if name.lower() not in constraint_name:
+                    col = rs[1]
+                    if rs[3] == 'BITMAP':
+                        idx_type = 'bitmap'
+                    elif rs[2] == 'UNIQUE':
+                        idx_type = 'unique'
+                    else:
+                        idx_type = ''
+                    ss = 'create ' + idx_type + ' index ' + user_upper + '.' + name.upper() + ' on ' + all_tablename_upper + ' (' + col.replace(' asc', '').replace(',', ', ') + ');' 
+                    mess = mess + ss + '\n'
+        
+        if not simple_mode:
+            # 建注释
+            sql = '''
+                select column_name, comments
+                from dba_col_comments
+                where owner = ? 
+                and table_name = ? 
+                and comments is not null
+            '''
+            mess = mess + '-- 注释' + '\n'
+            for r in ora_conn.run(sql, (username, table)).get_rows(True):
+                mess = mess + "comment on column " + all_tablename_upper + "." + r[0].upper() + " is '" + r[1] + "';\n"
+                
+        return Tools.merge_spaces(mess).strip('\n') 
+    
+    @staticmethod
     def get_table_size(dba_conn, username, table):
         """得到一个表相关对象的容量分布情况"""
         sql = '''
             select t.owner owner
                   ,t.segment_name table_name
                   ,t.segment_name obj_name
                   ,t.segment_type "TYPE"
@@ -687,7 +850,25 @@
                     # print(rep2kafka_info)
                     
         return ogg_info
 
 
 if __name__ == '__main__':
     main()
+    
+'''
+alter system set sga_max_size=18g scope=spfile;
+alter system set sga_target=18g scope=spfile;
+alter system set pga_aggregate_target=6g scope=both;
+alter system set "_partition_large_extents"=false scope=both sid='*';
+alter system set "_index_partition_large_extents"=false scope=both sid='*';
+alter system set audit_trail=false scope=spfile;
+alter profile default limit password_grace_time 9999;
+alter profile default limit password_life_time unlimited;
+alter profile default limit password_verify_function null;
+alter profile default limit password_reuse_max unlimited;
+alter profile default limit password_reuse_time unlimited;
+alter system set processes=6000 scope=spfile;
+alter system set sessions=6605 scope=spfile;
+alter system set db_recovery_file_dest_size='9999999G';
+alter system set enable_goldengate_replication=true scope=both;
+'''
```

### Comparing `tools_hjh-2.5.4/tools_hjh/SSHConn.py` & `tools_hjh-2.5.5/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/ThreadPool.py` & `tools_hjh-2.5.5/tools_hjh/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.4/tools_hjh/Tools.py` & `tools_hjh-2.5.5/tools_hjh/Tools.py`

 * *Files identical despite different names*

