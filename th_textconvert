# converter.py
import datetime
import os

def convert_utf8_to_ascii(dfile, sfile):
    with open(dfile,'w',encoding='tis-620') as w:
        with open(sfile,'r',encoding='utf-8') as r:
            data = r.read()
            w.write(data)
            
def convert_ascii_utf8(dfile, sfile):
    with open(dfile,'w',encoding='utf-8') as w:
        with open(sfile,'r',encoding='tis-620') as r:
            data = r.read()
            w.write(data)
            
def main():
    # convert utf-8 to ascii
    destfile = r'จังหวัดไทย-ascii.txt'
    sourcefile = r'จังหวัดไทย-UTF8.txt'
    fname, ext =os.path.splitext(sourcefile)
    today = datetime.datetime.now().strftime('%Y-%m-%d')
    convert_utf8_to_ascii(f'{fname}2ascii_{today}{ext}', sourcefile)
    # convert ascii to utf-8
    destfile = r'จังหวัดไทย-UTF8.txt'
    sourcefile = r'จังหวัดไทย-ascii.txt'
    fname, ext =os.path.splitext(sourcefile)
    today = datetime.datetime.now().strftime('%Y-%m-%d')
    convert_ascii_utf8(f'{fname}2UTF-8_{today}{ext}', sourcefile)
    
if __name__ =='__main__':
    main()
