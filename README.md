# coco2voc_changeLabel

1. python coco2voc.py -d <json文件> -s <保存转换为xml数据的文件夹>

2. 在文件中修改字符串： 
   if (sku.text == 'preName'):               #‘preName’为修改前的名称
                        sku.text = 'TESTNAME'                 #‘TESTNAME’为修改后的名称
                        tree.write(file,encoding='utf-8')     
           
if __name__ == '__main__':
    inputpath = '<路径>'  #此处替换为自己的路径
    changelabelname(inputpath)
