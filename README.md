# CSV处理
## 1.显示列名
> df.columns.to_list() #把列名转换为list
## 2.查看信息，了解列表
df.describe()
df.info()
df.memory_usage()
## 3.建立data_row \clean\analysis文件存档，以防万一
'''
path = os.path.join('data','raw') # A default location to save raw data
fn   = url.split('/')[-1]         # What does this do?
print(f"Writing to: {fn}")
if not os.path.exists(path):      # And what does *this* do?
    print(f"Creating {path} under {os.getcwd()}")
    os.makedirs(path)
    
df.to_csv(os.path.join(path,fn), index=False)
print("Done.")
'''

